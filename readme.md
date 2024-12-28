# Create pg
npm init -y
npm install node-pg-migrate pg

# Create migrate comments
npm run migrate create table comments

# Create migrate rename
npm run migrate create rename contents to body

# Create Table
DATABASE_URL=postgres://postgres:AnselZorro@localhost:5432/socialnetwork npm run migrate up

# Drop Table
DATABASE_URL=postgres://postgres:AnselZorro@localhost:5432/socialnetwork npm run migrate down