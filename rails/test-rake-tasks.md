```
require 'spec_helper'
require 'rake'

describe 'db:seeds' do
  before { MyApp::Application.load_tasks }

  it { expect { Rake::Task['products:load'].invoke }.not_to raise_exception }
end
```
