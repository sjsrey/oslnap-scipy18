# Spatio-temporal analysis of socioeconomic neighborhoods 


## Neighborhoods Matter

- neighborhood effects 
- gentrification
- community development

## Approaches to Neighborhoods

- neighborhood effects
  - massive literature
    - predictive postcode 
  - neighborhoods as "containers"
- neighborhood dynamics
  - process based models
  - prescriptive models
  - descriptive (exploratory models)


## (Temporal) Neighborhood Analysis Challenging

- what defines a neighborhood?
- "neighborhoods" change over time
    - compositionally
    - geographically/geometrically


## the Python ecosystem is ripe for neighborhood analysis

- pysal ecosystem
- geopandas
- scikit
- interactive viz and dashboard tools (that investors in Smart Cities *love*)

---

# Introducing The Open Source Longitudinal Neighborhood Analysis Package (OSLNAP)

- Data
- Analytics
- Visualization (note that we're still working on this piece so wont be talking about it much)



# Data Layer

We have Pandas, Geopandas, PySAL... why another data reader/manipulator?

- a common problem in neighborhood analysis is that enumeration units for survey datasets (e.g. the Census) change over time
- in other words, there is no consistent, **stable unit** to analyze over time
- spatial units cannot be subset without incurring unknown error (MAUP)


## picture of single big opaque census tract on a satellite image


## same tract but translucent, showing uneven development patterns underneath

(speaker explains point is that we can't naively assign statistics to arbitrary geographies, we need special tools to do that)

in the data module we provide tools to solve that problem in one of three ways:

- importing pre-standardized dataset from common provider
- providing statistical tools for harmonizing data to the spatial unit of the user's choice
- allowing the user to develop their own spatial units


## Import from external timeseries databases

[picture of logos from each of 3 providers]

(speaker describes how these are cleaned for common issues, standardized into consistent format, cached and optimized for modeling & viz)


## Harmonize/standardize new datasets to common boundaries

[ not sure the visual here ]


## Develop new primitive spatial units

[picture of intersection operation that creates small units]

(speaker describes how we use spatial statistical methods to develop reasonable estimates of the statistics within these units)

----

# Analytics I:  Identifying Neighborhoods


## Scientific Tradition

- briefly describe the SAA/FA/Geodemographics lineage, that social scientists
have long tried to identify neighborhoods based on their social characteristics. 

## [chicago school diagram]

(speaker explains that the concept is 100 years old, but we have better statistics for identifying the same kinds of patterns but they are difficult to use. that's one of the voids we fill. we also let researchers examine how these lines blur and shift over time)

## Current Art: Geodemographics

- use cluster analysis to derive neighborhoods
- commercial example?
-

## Enhancements

- we extend geodemographics to the temporal case
- we integrate new spatially explicit clustering algorithms

## [skater image]


## [spenc image]


# Analytics II:  Measuring Neighborhood Change

## Markov-Based Approaches

## Sequence Analysis

# Viz Teaser?
- solicit interest from collaborators?

# Conclusion
