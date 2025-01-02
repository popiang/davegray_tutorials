steps lesson 02

1. create the base code as usual for redux project
2. create the store
3. create the postsSlice
4. create PostsList.jsx to display the list
5. create AddPostForm.jsx to add post
6. create usersSlice.js
7. create PostAuthor.jsx
8. create TimeAgo.jsx
9. create ReactionButtons.jsx

steps lesson 03

1. install axios
2. set the POSTS_URL
3. create initialState
4. create fetchPosts
5. create extraReducers
6. export the state values
7. update PostList.jsx
   - get all posts values from postsSlice.js
   - use useEffect to fetchPosts using dipatch when postsStatus is idle
   - create variable content
   - update content based on postsStatus
   - create PostsExcerpt
7. create addNewPost
8. update extraReducers
9. update AddPost.jsx
   - update canSave, add checking if the status is idle
   - if canSave, call dispatch -> call addNewPost, unwrap, then, catch
10. in usersSlice.js
   - create USERS_URL const
   - create initialState emptry array
   - create fetchUsers
   - create extraReducers
   
