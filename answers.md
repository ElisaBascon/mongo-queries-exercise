# Solutions sheet

Submit your final query after each iteration:

## Iteration 1
db.users.find({}, {_id: 0, name: 1 })

## Iteration 2
db.users.find( { hasInsurance: { $ne: false } } )

## Iteration 3
db.users.find( { age: { $gte: 18 } } )

## Iteration 4
db.users.findOne( { country: { $eq: 'Italy' }}, {_id: 0, name: 1, email: 1} )

## Iteration 5
db.users.find( { country: { $eq: 'USA' }}, {_id: 0, name: 1}).limit(5)

## Iteration 6 
db.users.find( { phone: { $exists: true }})

## Iteration 7
db.users.updateOne( { email: "marissa@doe.com" }, {$set: {email: "marissa@hotmail.com"}})

## Iteration 8
db.users.updateMany( { country: "UK" }, {$set: { currency: "pounds"}})

## Iteration 9
db.users.find( { country: { $eq: 'UK' }}, {_id: 0, name: 1, currency: 1} )

## Iteration 10
db.users.deleteMany( { age: { $gte: 45 }})