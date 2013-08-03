### Update object based on relationship changes

adding :touch => true to a relationship declaration means that the associated thing will have its timestamps updated whenever 'this' class is saved.

example:


```ruby
class Foo < ActiveRecord::Base
  belongs_to :bar, :touch => true
end
```

means that when a Foo is saved then the Bar it belongs to will also have its timestamps updated.