// allow update: if isValidProduct();

function isValidProduct() {
  return incomingData().price > 10 && 
         incomingData().name.size() < 50 &&
         incomingData().category in ['widgets', 'things'] &&
         existingData().locked == false && 
         getUserData().admin == true
}
