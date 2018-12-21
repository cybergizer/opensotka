### Github username

@ARtoriouSs

### Link to Pull Request

1. https://github.com/spree-contrib/spree_slider/pull/42

### Short Description

Spree-slider is a Spree extension which provides an easy way to add customized slider to the shop.

When I install this extension, I found out that it's migrations fall with an error which says 'Add versions to your migrations!!1'. I google about it and found out that migration versions became required in Rails 5.1, but before Rails 5.0 they wasn't supported and this extension use migrations withot versions. So simple add versions to migrations will not be a right way to fix this problem, because it will fall on older Rails versions. But there is a pretty solution for this in Spree: it has its own migration class that require version, but it appends just if Rails version >= 5.1, so here I just inherit all migrations from this class.

This PR is open, but not merged yet.
