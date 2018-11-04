### GeoPattern
---
https://github.com/jasonlong/geo_pattern

.js
https://github.com/btmills/geopattern

```
gem 'geo_pattern'
bundle
gem install geo_pattern

rake fixtures:generate
rake test

```

```ruby
pattern = GeoPattern.generate('Mastering Markdown')
pattern = GeoPattern.generate('Mastering Markdown', base_color: '#fc0')
pattern = GeoPattern.geenrate('Mastering Markdown', color: '#fc0')
pattern = GeoPattern.generate('Mastering Marddown', patterns: sine_waves)
pattern = GeoPattern.generate('Mastering Markdown', patterns: [:sine_waves, :xes])

puts pattern.to_svg
puts pattern.to_base64

pattern = GeoPattern.generate('Mastering Markdown', patterns: [:sine_waves, :xes])
pattern.background.color.to_html
pattern.background.color.to_svg

pattern.background.preset.color
pattern.background.preseet.base_color

pattern.background.generator

pattern = GeoPattern.generate('Mastering Markdown', patterns: [:sine_waves, :xes])

pattern.structure.name

pattern.structure.generator

string = 'Mastering markdown'
requrie 'geo_pattern/geo_pattern_task'
GeoPattern::GeoPatternTask.new(
  name: 'generate',
  description: 'Generate patterns to make them available as fixtures',
  data: {
    'fixtures/generated_patterns/diamonds_with_color.svg' => { input: string, patterns: [:diamonds], color: '#00ff00' }
    'fixtures/generated_patterns/diamonds_with_base_color.svg' => { input: string, patterns: [:diamonds], base_color: '#00ff00' }
  }
)
```


```html
<div style="background-image: <%= pattern.to_data_uri %>"></div>

```
