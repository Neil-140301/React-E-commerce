

### Refer to image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authorisation-output-v2.gif" alt="nxt-trendz-authorisation-desktop-output" style="max-width:90%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>



#### App Functionality

The app has the following functionalities

- When an unauthenticated user tries to access the `HomeRoute`, `ProductsRoute`
  or `CartRoute` then the page should be redirected to the `LoginRoute`.
- When an authenticated user tries to access the `HomeRoute`, `ProductsRoute` or
  `CartRoute` then the page should be navigated to the respective route.
- When an authenticated user tries to access the `LoginRoute` then the page
  should be redirected to the `HomeRoute`.
- When the Logout button is clicked then the page should be navigated to the
  `LoginRoute`.
- When an undefined path is provided in the URL then the page should navigate to
the `NotFoundRoute`
</details>

<details close>
<summary>Click to view the Example response</summary>
<br>

- Success response from the URL `https://apis.ccbp.in/login` will be

```json
{
  "jwt_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InJhaHVsIiwicm9sZSI6IlBSSU1FX1VTRVIiLCJpYXQiOjE2MTk2Mjg2MTN9.nZDlFsnSWArLKKeF0QbmdVfLgzUbx1BGJsqa2kc_21Y"
}
```

- Failure response from the URL `https://apis.ccbp.in/login` for an invalid
  username will be

```json
{
  "status_code": 404,
  "error_msg": "Username is not found"
}
```

</details>



