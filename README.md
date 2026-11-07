# Exact enumeration of closed meanders

**Efthimios Alepis** · [ORCID 0000-0002-3862-7218](https://orcid.org/0000-0002-3862-7218) · [OEIS A005315](https://oeis.org/A005315)

This page is the single entry point for two **distinct approaches** to computing the closed meandric numbers $M_n$. The implementations, source histories, numerical records, and validation scopes remain separate. A modular check that shares an algorithm's structural code is not an independent proof of that structure.

## The two approaches

| Approach | Source and documentation | Scope of the cited release |
| --- | --- | --- |
| **C5/V2 transfer** | [Checked C5/V2 repository](https://github.com/talepis/meander-checked-c5-v2) · [archived release DOI](https://doi.org/10.5281/zenodo.23687622) | Exact CPU computation and retained records through $M_{34}$. The fast V2 memory bound is a *checked prediction*: a failed check triggers a retry with a proved cap. The release includes a separate original-transfer modular audit for $M_{29}$–$M_{31}$; the $M_{32}$–$M_{34}$ modular records share C5/V2 mathematics. |
| **Tree / bitmap geometry** | [Tree and bitmap repository](https://github.com/talepis/meander-tree-bitmap) | A different representation based on weighted tree/centroid states, frontier geometry, and bitmap supports. The cited release contains exact results for $M_{35}$–$M_{38}$, with [source, per-stage records, and validation details](https://github.com/talepis/meander-tree-bitmap/blob/main/docs/VALIDATION.md). Its modular checks for $M_{35}$–$M_{37}$ share structural components with the exact computation. No CRT check for $M_{38}$ is claimed. |

Both approaches enumerate the same sequence. Their differing representations should not be conflated, and the validation of one release should not automatically be attributed to the other. The public records document the scope and limitations of each check; they do not constitute institutional certification or a formal proof of every software execution path.

## Sequence data and provenance

- [Candidate b-file through $n=38$](https://github.com/talepis/meander-tree-bitmap/blob/main/oeis/b005315.txt). The OEIS draft is subject to editorial review; a candidate file is not an accepted extension by itself.
- [C5/V2 method, proofs, and CRT records](https://github.com/talepis/meander-checked-c5-v2).
- [Tree/bitmap method, results, and numerical audit](https://github.com/talepis/meander-tree-bitmap).
- Vladimir Osipov's earlier $M_{29}$ and $M_{30}$ contribution is documented in [his record](https://doi.org/10.5281/zenodo.22773575) and acknowledged in the [tree release's related work](https://github.com/talepis/meander-tree-bitmap/blob/main/docs/RELATED_WORK.md). No priority for those terms is claimed here.

To cite a computational method, cite its specific repository and release record. This landing page is for navigation and is not a third numerical implementation or a new validation claim.

The text on this page is released under the [MIT license](LICENSE).

