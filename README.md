# Postman Collection and Environment Configs for 8.3 API Testing

For more detailed and up-to-date info - https://docs.google.com/document/d/1N57QN-hUQGaT7IxcJAGUU2Wy7wgmxbnk_33ptxJn_Bg/edit?usp=sharing

Collection and environment configs for the new 8.3 API routes (RFC-68) can be imported in Postman for testing.

#### Usage
1. Import Collection config file in Postman.
2. Batch import environment configs.
3. On the `8.3` Collection parent level, navigate to Collection variables.
	- Set the desired target gateway address as necessary (default is http://localhost:8088).
      - Generate an API token on the test gateway and update the `api_token` variable
        - Note that `external` is preferred over `core` to better persist the token as the latter may be modified/cleared often by gwbk restores and/or manually.