use('restaurant');

db.restaurant.find();
db.restaurant.find({}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1});
db.restaurant.find({}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1, _id: 0});
db.restaurant.find({}, {restaurant_id: 1, name: 1, borough: 1, "address.zipcode": 1, _id: 0});
db.restaurant.find({borough: "Bronx"});
db.restaurant.find({borough: "Bronx"}).limit(5);
db.restaurant.find({borough: "Bronx"}).skip(5).limit(5);
db.restaurant.find({"grades.score": {$gt: 90}});
db.restaurant.find({"grades.score": {$gt: 80, $lt: 100}});
db.restaurant.find({"address.coord.0": {$lt: -95.754168}});
db.restaurant.find({{$and: [{ "cuisine": { $ne: "American" } }, { "grades.score": { $gt: 70 } },{ "address.coord.0": { $lt: -65.754168 } }]}});
db.restaurant.find({"cuisine": { $ne: "American" },"grades.score": { $gt: 70 },"address.coord.0": { $lt: -65.754168 }});
db.restaurant.find({"cuisine": { $ne: "American" },"grades.grade": "A","borough": { $ne: "Brooklyn" }}).sort({cuisine: -1});
db.restaurant.find({"name": /^Wil/}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1, _id: 0});
db.restaurant.find({"name": /ces$/}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1, _id: 0});
db.restaurant.find({"name": /.*Reg.*/}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1, _id: 0});
db.restaurant.find({borough: "Bronx", $or: [{cuisine: "American "}, {cuisine: "Chinese"}]});
db.restaurant.find({$or: [{borough: "Staten Island"}, {borough: "Queens"}, {borough: "Bronx"}, {borough: "Brooklyn"}]}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1, _id: 0});
db.restaurant.find({$nor: [{borough: "Staten Island"}, {borough: "Queens"}, {borough: "Bronx"}, {borough: "Brooklyn"}]}, {restaurant_id: 1, name: 1, borough: 1, cuisine: 1, _id: 0});
db.restaurant.find({"grades.score": {$not: {$gt: 10}}});




