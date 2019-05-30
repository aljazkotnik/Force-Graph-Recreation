# Force-Graph-Recreation
Setting up a working version in preparation for using own data


Data:
- miserables.json - the Les Miserables data taken from a d3 example page.
- testData2.json - literature review data formatted in the "miserables.json" format, but with added node size options. The node sizes are the connections of the node, specifically the number of articles that it cites.

Code:
- miserables.html - the original force graph chart representing the connections of characters in te novel Les Miserables. The chart offers some insights into the story: Distinct groups are present inthe story, and not all interact with all (e.g. no orange/dark blue connection). There are several ring leaders, most notably Valjean, Marius, Gavroche, Enjolras, and Fantine. These characters are the main links between their groups and the rest of the cast. Notice that Javert, although the principal antagonist in the story, is not a ring leader, which could potentially mean that the novel rarely places him in a non-confrontational scene, therefore potentially reducing the understanding of the character.

- litReview.html - the very basic force graph chart of half the references found. Several clusters of articles can be seen. These are the "vortex", "shock-wave", "oceanic", "coherent-structures" clusters. Several isolated items are also present. These could be color coded, and the code supports easy implementation of this. The grouping must be done by the user however. This could potentally be done automatically by Latent Dirichlet algorithms, which would find appropriate descriptos for the clusters. Date of publication is not present, but important, as it allows to trace the ideas to their inception. Date could be introduced as a color code. This could be selected using a switch, or the node shapes could be changed to maintain the distinction between clusters.

- litReview2.html - an upgrade from "litReview", it uses the amount of it's connections to determine the node size. This allows to identify the articles that cite the most others. This can help find the most instructive articles. A switch between node sizing/no node sizing should be incorporated.
