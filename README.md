# cg-deploy-paas-billing
Concourse Pipeline to deploy paas-billing in cloud.gov

## Customizing the frontend

Put frontend customization directions here...

### Get dependencies

Put dependencies here...

### Deploy the backend to your cloud.gov sandbox

May not be needed...

### Create a service instance user so you can login

- Create a service instance of the `cloud-gov-service-account` service, called
  `paas-billing-account`, using the `space-auditor` plan/role
  ```
  cf create-service cloud-gov-service-account space-auditor paas-billing-account
  ```
- Create a service key tied to that instance
  ```
  cf create-service-key paas-billing-account paas-billing-account-creds
  ```
- Get a copy of the credentials so you can login later
  ```
  cf service-key paas-billing-account paas-billing-account-creds
  ```

### Modify frontend configuration

Put frontend modification directions here...


### Run the frontend

Put frontend run instructions here...


## Contributing

See [CONTRIBUTING](CONTRIBUTING.md) for additional information.

## Public domain

This project is in the worldwide [public domain](LICENSE.md). As stated in
[CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and
> copyright and related rights in the work worldwide are waived through the
> [CC0 1.0 Universal public domain
> dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0
> dedication. By submitting a pull request, you are agreeing to comply with
> this waiver of copyright interest.
