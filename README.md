### camping
---
https://github.com/camping/camping

```ruby
require 'camping'
Camping.goes :Blog
module Blog::Models
  class Post < Base; belogs_to :user; end
  class Comment < Base; belongs_to :user; end
  class User < Base; end
end
module Blog::Controllers
  class Index
    def get
      @post = Post.find :all
      render :index
    end
  end
end
module Blog::Views
  def layout
    head { title "My Blog" }
    body "My Blog"
      h1 "My Blog"
      self << yeild
    end
  end
  def index
    @posts.each do |post|
      h1 post.title
    end
  end
end

class CreateTheBasics < V 0.1
  def self.up
    create_table Page.table_name do |t|
    end
  end
  def self.down
    drop_table Page.table_name
  end
end

secret "Very secret text, which no-one else should know!"

def r501(method)
  "Sorry, but I can't respond to #{method}"
end
def r500(klass, method, ex)
  "Sorry, but #{klass}##{method} failed with #{ex}."
end

```

```sh
gem install camping
gem install camping-omnibus --source http://gems.judofyr.net
gem install markaby
gem install activerecord
```

```
```


