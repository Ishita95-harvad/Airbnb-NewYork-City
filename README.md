**1. Airbnb**

**An example of an A/B test**

In addition, A/B testing requires the building of additional infrastructure to support the ability to serve different models to different users. Let’s cover each of these challenges in more detail.

**Choosing groups and duration**

Deciding which users should be served which model comes with a few requirements. Users in both groups should be as similar as possible so that any observed difference in outcome can be attributed to our model and not to a difference in cohorts. If all users in group A are power users and group B contains only occasional users, the results of an experiments will not be conclusive.

In addition, the treatment group B should be large enough to draw a statistically meaningful conclusion, but as small as possible to limit exposure to a potentially worse model. The duration of the test presents a similar trade-off: too short and we risk not having enough information, too long and we risk losing users.

These two constraints are challenging enough, but consider for a minute the case of large companies with hundreds of data scientists who run dozens of A/B tests in parallel. Multiple A/B tests may be testing the same aspect of the pipeline at the same time, making it harder to determine the effect of an individual test accurately. When companies get to this scale, this leads them to building experimentation platforms to handle the complexity. See Airbnb’s ERF, as described in Jonathan Parks’s article, “Scaling Airbnb’s Experimentation Platform”; Uber’s XP as described in A. Deb et al.’s post, “Under the Hood of Uber’s Experimentation Platform”; or the GitHub repo for Intuit’s open source Wasabi
