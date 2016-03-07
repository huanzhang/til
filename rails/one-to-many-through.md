```
class Employment < ActiveRecord::Base
  belongs_to :employee  # foreign key - programmer_id
  belongs_to :company     # foreign key - project_id
end
class Employee < ActiveRecord::Base
  has_one :employment
  has_one :company, :through => :employment
end
class Company < ActiveRecord::Base
  has_many :employments
  has_many :employees, :through => :employments
end
```
