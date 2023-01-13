# -react-hooks-jwt-auth-snippet
About React Hooks JWT Auth using React code snippets


### Note:
Open `src/services/auth-header.js` and modify `return` statement for appropriate back-end 

```js
export default function authHeader() {
  const user = JSON.parse(localStorage.getItem('user'));

  if (user && user.accessToken) {
    // return { Authorization: 'Bearer ' + user.accessToken }; // for Spring Boot back-end
    return { 'x-access-token': user.accessToken };             // for Node.js Express back-end
  } else {
    return {};
  }
}
```


## React app package.json file

| | | | | | | | | | | | | | | | | | | | | |
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|name|version|private|dependencies| | | | | | | | | | |scripts| | | |eslintConfig|browserslist| |
| | | |@testing-library/jest-dom|@testing-library/react|@testing-library/user-event|axios|bootstrap|react|react-dom|react-router-dom|react-scripts|react-validation|validator|start|build|test|eject|extends|production|development|
|react-hooks-jwt-auth|0.1.0|TRUE|^5.14.1|^11.2.7|^12.8.3|^0.26.1|^4.6.0|^17.0.2|^17.0.2|^6.2.2|4.0.3|^3.0.7|^13.0.0|react-scripts start|react-scripts build|react-scripts test|react-scripts eject|react-app|&gt;0.2%|last 1 chrome version|
| | | | | | | | | | | | | | | | | | | |not dead|last 1 firefox version|
| | | | | | | | | | | | | | | | | | | |not op_mini all|last 1 safari version|
