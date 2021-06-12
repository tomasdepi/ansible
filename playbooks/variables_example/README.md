# Variables Priority

1. Default (defined within the role)
2. Group variables (var_groups/all, var_groups/\<group\>)
3. Host variables (var_hosts/\<host\>)
4. Facts of the server
5. Server's variables (var_prompt, var_files)
6. Role's variables (defined in roles/role/var/main.yml)
7. Block variables
8. Role's parameters (include_params, include_vars)
9. set_factes, registered_vars
10. extra_vars