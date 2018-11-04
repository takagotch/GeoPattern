### GeoPattern
---
https://github.com/jasonlong/geo_pattern

.js
https://github.com/btmills/geopattern

```
gem 'geo_pattern'
bundle
gem install geo_pattern

```

```ruby
pattern = GeoPattern.generate('Mastering Markdown')
pattern = GeoPattern.generate('Mastering Markdown', base_color: '#fc0')
pattern = GeoPattern.geenrate('Mastering Markdown', color: '#fc0')
pattern = GeoPattern.generate('Mastering Marddown', patterns: sine_waves)
pattern = GeoPattern.generate('Mastering Markdown', patterns: [:sine_waves, :xes])

puts pattern.to_svg
puts pattern.to_base64


```


```html
<div style="background-image: <%= pattern.to_data_uri %>"></div>

```
