## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/36

**Issue title:** Architecture doc doesn't explain the hybrid retrieval scoring formula

**Tier:** [x] Tier 1  [ ] Tier 2  [ ] Tier 3

**Problem summary:**
The architecture documentation explains that PathReview combines vector-search and keyword-search results during hybrid retrieval, but it does not show how the two scores are mathematically combined. It also omits the default weighting assigned to each retrieval method, making it difficult for contributors to understand or reason about the final ranking. This issue affects `docs/ARCHITECTURE.md`, although the implementation must also be reviewed to ensure the documentation matches the actual retrieval behavior. A successful fix will add the scoring formula, identify the default weights, and include a worked example showing how a final hybrid score is calculated.

**Selection notes — “Is this right for me?” checklist:**
This issue has a clearly defined documentation deliverable and is limited primarily to one file. The necessary information should be available in the hybrid retrieval implementation, so the scope can be verified before making changes. I am comfortable reading Python code and translating implementation details into clear technical documentation. The issue does not require redesigning the retrieval system or changing application behavior, and its estimated effort of two to three hours fits the module timeline.

**Branch name:** docs/36-explain-hybrid-retrieval-scoring

**Setup confirmation:** [yes] App runs locally at localhost:5173

**Cohort ledger:** [ yes] Issue added to cohort ledger
