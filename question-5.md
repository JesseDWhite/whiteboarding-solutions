function sortArray(array) {
  let complete = false;
  while(!complete) {
    complete = true;
    for (let i = 1; i < array.length; ++) {
      if (array[i - 1] > array[i]) {
        complete = false;
        let temp = array[i -1];
        array[i - 1] = array[i]
        array[i] = temp;
      }
    }
  }
  return array;
}