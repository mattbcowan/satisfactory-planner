# Satisfactory Planner

## API

| Endpoint         | Functionality                                                                           | Public or Private | Parameters                          | Returns                                                                                                                               | Notes |
| ---------------- | --------------------------------------------------------------------------------------- | ----------------- | ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Users            | Create a user, edit a user, retrieve a user, reset a password, view profile, view plans | Public            | user_id                             |                                                                                                                                       |       |
| Plans            | Create a plan, edit a plan, retrieve a plan, reset a plan, delete a plan                | Public            | plan_id                             |                                                                                                                                       |       |
| Buildings        | Retrieve a building                                                                     | Public            | building_id                         | building_id, inputs, outputs, recipes, overclock_bool, clock_percent, power_usage, width, length, height, area, ingredients, category |       |
| Components       | Retrieve a component                                                                    | Public            | component_id                        | component_id, stack_size, sink_value, recipes, ingredients, building_needed, category                                                 |       |
| Resources        | Retrieve a resource                                                                     | Public            | resource_id                         | resource_id, stack_size, sink_value, node_type, building_needed, recipes                                                              |       |
| Calculate Output |                                                                                         | Private           | multiple inputs of building outputs | total_output                                                                                                                          |       |

Note: Double check Private VS Public endpoints to be sure these are correct.

## Backend Stack

Express - Restful API

JEST - Testing

MongoDB - Database

Mongoose - Modeling
