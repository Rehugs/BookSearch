# Book Searcher

Easy and blazing-fast book searcher, create and search your private library.

Book Searcher can index metadata for over 10 million books in one minute, and search in 30µs.

### Deploy with Vercel

<div align=center>

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/Rehugs/BookSearch/tree/master/&project-name=book-search&repository-name=book-search)

</div>

Deploying the frontend to Vercel to speed up loading of static resources and provide a reverse proxy to the image service.

### Original Search Api

You can search by the following fields:

- title
- author
- publisher
- extension
- language
- isbn
- id

Examples:

- `/search?limit=30&offset=0&title=TITLE`
- `/search?limit=30&offset=0&title=TITLE&author=AUTHOR`
- `/search?limit=30&offset=0&isbn=ISBN`
- `/search?limit=30&offset=0&query=title:TITLE extension:epub publisher:PUBLISHER`

We now have two search modes, `/search?limit=30&offset=0&mode=explore&title=TITLE&author=AUTHOR`

- filter: the results need to meet all restrictions, default mode
- explore: the results only need to meet certain restrictions

## License

**book-searcher** © [The Book Searcher Authors](https://github.com/book-searcher-org/book-searcher/graphs/contributors), Released under the [BSD-3-Clause](./LICENSE) License.