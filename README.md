# assertive.data.uk

A set of predicates and assertions for checking the properties of UK-specific complex data types.  Most of the documentation is on the *[assertive](https://bitbucket.org/richierocks/assertive)* page.  End-users will usually want to use *assertive* directly.


### Installation

To install the stable version, type:

```{r}
install.packages("assertive.data.uk")
```

To install the development version, you first need the *devtools* package.

```{r}
install.packages("devtools")
```

Then you can install the *assertive.data.uk* package using

```{r}
library(devtools)
install_bitbucket("richierocks/assertive.data.uk")
```

### Predicates

`is_uk_car_licence` checks character vectors for UK car licence plates.

`is_uk_national_insurance_number` checks character vectors for UK National 
Insurance numbers.

`is_uk_postcode` checks character vectors for UK postcodes.

`is_uk_telephone_number` checks character vectors for UK telephone numbers.

### Assertions

Predicates all return a vector and have two corresponding assertions.  For example,
`is_uk_car_licence` has `assert_all_are_uk_car_licences` and `assert_any_are_uk_car_licences`.
