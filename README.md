# Sequelize CLI, Associations

```bash
# install Sequelize globally
yarn global add sequelize-cli
# make sequelize name shorter its hard to type
alias seq="sequelize "

# creating working folder 
mkdir sequelized
cd sequelized
yarn init -y
yarn add sequelize, mysql2

# initialize the project with folder structure
seq init
seq db:drop
seq db:create
seq model:generate --name User --attributes firstName:string,lastName:string,email:string,password:string
seq db:migrate
# Now lets create a seed file:
seq seed:generate --name user
seq db:seed:all

# Defining associations
seq model:generate --name Task --attributes title:string,userId:integer

```
