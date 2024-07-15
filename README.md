const arr = [5, 6, 7, 8, 9, 2, 6, 3, -4, 0, -9, -6];
let filteredArr = [];
const myFilter = (element) => {
	if (element >= 0) {
		return true;
	}
	else {
		return false;
	}
}
arr.forEach(element => {
	if (myFilter(element) === false) {
		filteredArr.push(element);
	}
})

console.log("After filtering:", filteredArr);
