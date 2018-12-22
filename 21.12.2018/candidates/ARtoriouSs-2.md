### Github username

@ARtoriouSs

### Link to Pull Request

1. https://github.com/spree-contrib/spree_slider/pull/44

### Short Description

Spree-slider is a Spree extension which provides an easy way to add customized slider to the shop.

Another problem with Spree slider was in it's views, and specifically in ```image_tag```. When I install migrations and tried to open its views on admin panel, it falls again. After a little walk on the internet I found that Rails 5.2 changed behavior for ```image_tag``` and now it cannot accept image objects, you can only send URL. So I have fix this moment and send PR, but it's pending too :(
