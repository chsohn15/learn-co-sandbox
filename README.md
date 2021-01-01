
Hi! 👋

You've opened the IDE Sandbox, an environment that you can access on "readme" and "code-along" lessons in Learn. It's a great place to experiment with code! 🎉

*IMPORTANT*
Saving varies by the type of work you are doing:
-- Most of the work you do in the Sandbox is automatically saved on your behalf to the `learn-co-sandbox` repository in your GitHub account. Please DO NOT touch this repository in GitHub. Doing so will affect your Sandbox experience, and potentially cause your work to fall out of sync.
-- *Git repositories that you clone into the Sandbox are NOT automatically saved.* In this case, you are responsible for committing and pushing your work to GitHub. 

To learn more about the Sandbox, please visit http://help.learn.co/technical-support/learn-ide-in-browser/ide-in-browser-sandbox

1. Through validations, user_name uniqueness = true
2. user = User.new 
   if user.valid?
      user.save 
      redirect_to user_path(user)
   else 
      render :new   
3. index - > tweets/tweet_id/comments, show -> tweets/:id/comments/:id
4. Improve user experience, easier to navigate and find information, less clicking
5. a.) def index @tweets = Tweet.all end 
   view => tweets/index.html.erb => iterate through @tweets
   b.) def show # find tweet that fits params id
            tweets/show.html.erb => display @tweet information 
   c.) def comments  #find tweet, @all_comments = tweet.comments
          tweets/comments.html.erb -> display @all_comments
6. set_tweet finds the specific tweet based on the parameters
   tweet_params sets which parameters the create and update actions accept
7. tweet/edit.html.erb
  <% = form_for @tweet do |f| %>
  <%= f.label :content %>
  <%= f.text_field :content %>
  <%= f.submit %> 
  <% end %>

8.tweets/:tweet_id/comments/:comment_id/likes
  Show all the likes for one comment in one tweet_id
  

  
  TweetsController
  
  def index
  end
  
  ..
  
  def comments
    @comments = 














