//solution without using the filter() method
function unDoopArray(array) {
  let sortedArray = array.sort();
  for (let i = 0; i < sortedArray.length; ++) {
    if (i === i++) {
      sortedArray.splice(i, 1);
    }
  }
  return sortedArray;
}

//solution using the filter() method
function unDoopArray(array) {
  array.filter(word => word !== word);
  return array;
}