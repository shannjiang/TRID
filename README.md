# TRID
\name{TRID}
\alias{TRID}
\title{Calculation of gene TRID weights from a gene expression matrix}
\description{Calculate differential expression, differential connectivity and DiCODE (Differential COnnectivity and Differential Expression) weights of genes of any given gene expression matrix.}
\usage{
TRID(datExpr, datExpr_annotation, connectivity_method = NULL)
}
\arguments{
  \item{datExpr}{
the gene expression matrix used to compute TRID weights with columns correspond to individual genes and rows correspond to individual samples
}
  \item{datExpr_annotation}{
the annotation file with one column "status" which indicates two phenotypes of individual samples
}
  \item{connectivity_method}{
character, "pearson" (default) or "spearman" method used for calculation of differential connectivity
}
}
\value{
TRID(): Returns TRID weight lists
}
\author{
Shan Jiang
}
\examples{
# compute TRID weights
TRID_weights <- TRID(datExpr, datExpr_annotation)
}
% Add one or more standard keywords, see file 'KEYWORDS' in the
% R documentation directory.
\keyword{ ~kwd1 }
\keyword{ ~kwd2 }% __ONLY ONE__ keyword per line
