# Version 0.1.3

* ClusterMF is soft deprecated; it has the same functionality as 
  MetaForest. You can simply replace any call to ClusterMF with a call to
  MetaForest with the same arguments.
* A clustered MetaForest analysis no longer automatically doubles the number of
  trees estimated. Instead, it divides num.trees trees by two, rounding up to 
  the nearest even number.
* Generic S3 methods are now properly declared as such, instead of being 
  exported with their own documentation.
* Reduce dependencies by calculating partial dependence manually

# Version 0.1.2

* Rewrote WeightedScatter to jointly plot numeric and factor variables
* Rewrote PartialDependence to be an S3 generic, with methods for metaforest and
  rma models
* Rewrote PartialDependence to jointly plot numeric and factor variables
* Added ModelInfo_mf(), which returns a ModelInfo list for using metaforest with
  caret
* Added ModelInfo_rma(), which returns a ModelInfo list for using rma with caret

# Version 0.1.1

* Substantial update to PartialDependence
* PartialDependence now plots percentile interval for predictions
* PartialDependence now plots weighted raw data
* Improved speed of PartialDependence
* Improved speed of plot.MetaForest by vectorizing calculations
* Removed dependency on edarf
* Removed dependency on reshape2
* MetaForest and ClusterMF now return vi and weights vectors for plotting
* Improved speed of extract_proximity.MetaForest by using matrix operations
* Added WeightedScatter for weighted scatterplots of meta-analytic data
