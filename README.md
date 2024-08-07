
<!-- README.md is generated from README.qmd. Please edit that file -->

# ISF2024: Feature based graph pruning for improved forecast reconciliation

<!-- badges: start -->
<!-- badges: end -->

Slides and notes for a talk at the 44th International Symposium on
Forecasting (30th June - 3rd July 2024) in Dijon, France.

<!-- A recording of this presentation is available on YouTube here: <https://www.youtube.com/watch?v=FBM-nEbeHTw> -->
<!-- [![](preview.jpg)](https://www.youtube.com/watch?v=FBM-nEbeHTw) -->

#### Abstract

Large collections of related time series are commonly structured with
aggregation constraints, whereby each series possesses various
attributes that identify their relation to other series. These
attributes typically relate to what is being measured, such as product
categories or store locations for the sales of a product over time. When
there exists many attributes for time series data, the number of series
in the collection quickly becomes unmanageable with disproportionately
many uninformative disaggregated series. This presents many problems for
forecasting, since producing many forecasts can be computationally
infeasible and the forecast accuracy for aggregated series of interest
can worsen.

To overcome these problems I propose using time series features to
identify noisy, uninformative, or otherwise unwanted series and
leveraging the graph structure from topic 1 to safely remove them while
preserving coherency constraints. Pruning series from the bottom of the
structure would result in graph coherency constraints since a common
bottom level is no longer present. Various control points are possible,
including specification of features, thresholds, and coherent pruning
rules to produce a reduced set of coherent series for forecasting.
Pruning subgraphs of time series from the collection can substantially
reduce the number of series to forecast, while retaining most of the
information. This helps limit the computational complexity of
forecasting, while improving forecast accuracy for aggregated series due
to reduced model misspecification in more disaggregated series.

#### Structure

- Recap of graph reconciliation
- The curse of dimensionality in reconciliation, large scale and
  inaccurate (?)
- Feature-based pruning of coherency constraints for improved
  computational complexity and forecasting accuracy
- Application and evaluation on real example

### Format

17 minute talk with 3 minutes for questions.
