
RoR Udemy course details and notes
    1. A
    2. b
    3. c
    4. Web apps
       Ruby-lang and RoR- framework
       Databases- sqlite
    5. tryruby.org
    6. quiz
    7. IDE either c9 or codeanywhere
       install ruby, RVM, node and yarn(for js environmenti)
	ruby -v
	rails -v(using gems)
    12.Gem file-- contains all the dependencies
	bundle insall---> goes gem.org.ruby and installs in gem file
	app folder--> MVC/ assets--> styling/image
	config file--> db.yaml and routes(recieves reuest )
	classnames--> sneak_case-> CamelCase	
	migrations--> automatically but others write eerything
    13. Method--> action
	view--> application.html.erb--> all are in this
    14. rails new app_name	
	to run--> go to app_name: rails s 
	Create controllers in controller and inherit the ActionController
    16: For that controller, you should have that folder in views, which has .html.erb
	About routing... get '/about', to: "pages#view"
	gets displayed through layout "<yield>"
    18: CRUD operations
	Models--> interact DB with app'n
	Migrations--> deals with table (rails generate migraton create_todos)
	Controller--> todos_controller.rb (pl), Model--> todo.rb (class-todo),                     	   table-> todos table(plural)
	C - Create, R - Read, U - Update, D - Delete
	Standard database operations - CRUD

	Create a migration file to create todos table:
	rails generate migration create_todos

	Then within the change method under create_table, fill in the attribute details:
	t.string :name
	t.text :description

	Save this file and then run the migration:
	rails db:migrate

	To start the rails console:
	rails console

	To exit the rails console:
	exit
    20: rails console
	helps to interact w db and models
	lunch = todo.new[v1:"",v2:""]
	.new and .save
	.create--> directly save to DB
	.update or .find and change the field
	"validate" in models and keep checking
	reload! and todo3.errors.any? and todo3.errors.messages 
	resources:todos--> gives CRUD routes

	
Front-END interface
25:   	Creating a dashboard
	Under views, create a new folder called todos, and a new file under it called new.html.erb 		so in views/todos/new.html.erb file, fill in the new todo form:
	Create an instance variable in views in form @todo and define it in controllers

26: Creating a todo complete page
	The #new to ceate a table
	the #submit hits to db
	https://www.udemy.com/course/pro-ruby-on-rails-rails5/learn/lecture/6558560#announcements
28: Showing
	Using flash to preview messages
	T0do.find(params[:id])
30: Editing
	https://www.udemy.com/course/pro-ruby-on-rails-rails5/learn/lecture/6558628#announcements

32:Listing routes 

34: Destroying in CRUD operations of DB rom UI
	Refactoring code, adding commanalities by putting <%= render 'layouts/messages'%>

35:Deployed in hEroku
https://www.udemy.com/course/pro-ruby-on-rails-rails5/learn/lecture/6558672#announcements


