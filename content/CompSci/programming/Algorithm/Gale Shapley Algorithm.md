---
tags:
  - CompSci/programming/Algorithm
---
# Gale Shapley Algorithm
### Description:
- **Input:**
	* **Set A:** Set of proposers (e.g., men, students, residents)
	* **Set B:** Set of receivers (e.g., women, colleges, hospitals)
	* **preferences_A:** Preference lists for each proposer in A
	* **preferences_B:** Preference lists for each receiver in B
- **Output:**
	* **matching:** A stable matching between A and B
- **Function:** Gale-Shapley(Set A, Set B, preferences_A, preferences_B)
	1. **Initialize:**
	    * matching: An empty dictionary
	    * for each proposer a in A:
	        * a.partner = None
	    * for each receiver b in B:
	        * b.partner = None
	2. **While there exists a free proposer a in A:**
	    * Let b be the next receiver in a's preference list
	    * If b.partner is None:
	        * Set matching[(a, b)] = True
	        * Set a.partner = b
	        * Set b.partner = a
	    * Else:
	        * Let c be b.partner
	        * If b prefers a to c according to preferences_B[b]:
	            * Set matching[(a, b)] = True
	            * Set matching[(c, None)] = False **(break c's engagement)**
	            * Set a.partner = b
	            * Set b.partner = a
	        * Else:
	            * Do nothing (a stays unmatched)
---