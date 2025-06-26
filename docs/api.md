ase URL
https://dummyapi.io/data/v1/
Headers
It is required to set app-id Header for each request.
It helps us to determine your personal environment. So only you can access data that were created or update.

You can get personal App ID value on your account page.
You can have as much App ID as you want and use it in parallel(for different projects, envs etc).

Example: app-id: 0JyYiOQXQQr5H9OEn21312
Paging
For some endpoints you will get a single item. But for some of them it should be a list of objects.
To control amount of items, you need to use page and limit URL params.
Limit value should be in range [5-50]. Default value: 20
Page value should be in range [0-999]. Default value: 0

Example: https://dummyapi.io/data/v1/user?page=1&limit=10
Take 10 elements on a second page(page number starts from zero). Return items from 11 to 20 in a default order.
Created
In case you want to get only items created in current environment(exclude base items).
Use created query parameter - created=1.

Example: https://dummyapi.io/data/v1/user?created=1