 ## 10-sec Version
- Negative-binomial distribution with a common dispersion parameter is able to estimate the fraction of zeros in negative-control datasets for droplet scRNA-seq.
- Additional zero values in biological data are likely due to biological variation.

## My follow-up Question
- What is it mean to have gene wise dispersion parameter?
- If we believe the zeros out of the expectation of Negative Binomial is due to biological variation, is it biological noise or signal?
- What do we mean when we say biological variation?
- Knowing the underlying distribution gives us what advantage?

## Digest
 - Negative-control datasets have been generated by adding a solution of RNA to the fluid in microfluidic systems, making the RNA content in each droplet identical.
 - The negative-control data for droplet-based methods presented here indicate that the number of zero values observed is consistent with what is expected from count data. Additional zero values in biological data are likely due to biological variation.
 - Biological data display a larger number of zero values than expected for a homogenous populations of cells (Fig. [1f,g](https://www.nature.com/articles/s41587-019-0379-5#Fig1)) and, to an even larger degree, for heterogeneous populations of cells (Fig. [1h](https://www.nature.com/articles/s41587-019-0379-5#Fig1)). 
 - When allowing independent dispersion parameters for each gene, many of the zero values in biological data can be accounted for, whereas negative control data only show marginal improvements.

## Highlight Figure

![Fig. 1](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41587-019-0379-5/MediaObjects/41587_2019_379_Fig1_HTML.png)