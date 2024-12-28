# Create pg
npm init -y
npm install node-pg-migrate pg

# Create migrate comments
npm run migrate create table comments

# Create migrate rename
npm run migrate create rename contents to body

# Migrate up
DATABASE_URL=postgres://postgres:Password@localhost:5432/socialnetwork npm run migrate up

# Migrate down
DATABASE_URL=postgres://postgres:Password@localhost:5432/socialnetwork npm run migrate down

# Check Node
Node index.js