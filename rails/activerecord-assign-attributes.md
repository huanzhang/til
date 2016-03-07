Allows you to set all the attributes by passing in a hash of attributes with keys matching the attribute names (which again matches the column names).

```
cat = Cat.new(name: "Gorby", status: "yawning")
cat.attributes # =>  { "name" => "Gorby", "status" => "yawning", "created_at" => nil, "updated_at" => nil}
cat.assign_attributes(status: "sleeping")
cat.attributes # =>  { "name" => "Gorby", "status" => "sleeping", "created_at" => nil, "updated_at" => nil }
```
