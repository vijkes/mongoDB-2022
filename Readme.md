{
  "name": "keshav",
  "mob": 15465,
  "remark": "ok",
  "workactive": true
}

{
  name: "madhav",
  mob: 1546345,
  remark: "ok",
  workactive: false
}

{ name: "golu",  whatapp:  125465,  city: 'pune', salary: 43.2 },
{ name: "ajit",  hike:  5442 ,  city: 'Singhwara', salary: 47.4 },
{ name: "raj",  insta: "loving_boy",  city: 'Dbg', salary: 23.2, pay: "UPI" },
{ name: "malhotra",  pager:  4125465,  city: 'Goa', salary: 34.6, pay: "UPI" }

{
name: "paris",
email: "paris@paris.com",
country: "France"

}


	{
	name: "London",
	email: "paris@paris.com",
	country: "UK"

	},

	{
	name: "Berlin",
	email: "paris@paris.com",
	country: "Bercilia"

	}



/////////////////////////////////////////////////
db.students.find()

devbots> db.students.update({}, {$set: {workactive: false} } )


devbots> db.students.update({}, {$set: {workactive: true} } )
DeprecationWarning: Collection.update() is deprecated. Use updateOne, updateMany, or bulkWrite.
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 0,
  upsertedCount: 0
}

devbots> db.students.updateMany({}, {$set: {workactive: true} } )

devbots> db.students.updateOne({"country": "France"}, {$set: {"country": "Ukraine"} } )

devbots> db.students.findOne({"name": "golu"})

db.students.deleteOne({pay: "UPI"})

db.students.insertMany(
... [
... { name: "raj",  insta: "loving_boy",  city: 'Dbg', salary: 23.2, pay: "UPI" },
... { name: "malhotra",  pager:  4125465,  city: 'Goa', salary: 34.6, pay: "UPI" }
... ]
... )


db.students.deleteMany({whatapp: 125465})

db.students.insertOne({ name: "golu",  whatapp:  125465,  city: 'Bhilwara', salary: 43.2 })


db.students

use devbots
