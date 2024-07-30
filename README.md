# Postman Collection and Environment Configs for 8.3 API Testing

For more detailed and up-to-date info - [[Ignition 8.3 Early Access] 8.3 API - Postman Config](https://forum.inductiveautomation.com/t/8-3-api-postman-config-github/93935)

Collection and environment configs for the new 8.3 API routes can be imported in Postman for testing.

#### Usage
1. Import Collection config file in Postman.
2. Batch import environment configs.
3. On the `8.3` Collection parent level, navigate to Collection variables.
	- Set the desired target gateway address as necessary (default is http://localhost:8088).
      - Generate an API token on the test gateway and update the `api_token` variable
        - Note that the `data/config/EXTERNAL/ignition/api-token` directory location is preferred over `data/config/CORE/ignition/api-token` to better persist the token as the latter may be modified/cleared often by gwbk restores and/or manual intervention.