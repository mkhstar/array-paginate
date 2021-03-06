
# Array Paginate (array-paginate)

Array paginate is a library that takes in an array and paginate it to suit the needs of users.

## Installation

Use the package manager [npm] to install array-paginate.


```bash
npm install array-paginate
```
## Arguments
```javascript
arrayPaginate(array, page, limit)
```

| argument | type   | default   | description                                      |
|----------|--------|-----------|--------------------------------------------------|
| array    | Array  | undefined | The array of items that is to be paginated       |
| page     | Number | 1         | The page number to return from the pagination    |
| limit    | Number | 10        | The number of items to be returned for each page |

## Usage


```javascript

var arrayPaginate = require('array-paginate');
const array = ["first","second","third","fourth", "fifth"]
const paginatedItems = arrayPaginate(array, 1, 3);

console.log(paginatedItems);
//Returns
/*
{
	docs: ["first","second","third"],
	currentPage: 1,
	perPage: 3,
	total: 5,
	totalPages: 2,
	hasNextPage: true,
	hasPrevPage: false
}
*/
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.



## License
[MIT](https://choosealicense.com/licenses/mit/)
