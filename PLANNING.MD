# Satisfactory Planner

## API

| Endpoint | Functionality | Public or Private | Parameters | Returns | Notes |
| --- | --- | --- | --- | --- | --- |
| Users | Create a user, edit a user, retrieve a user, reset a password, view profile, view plans | Public | user_id |  | This will be added later if I decide to add in logging in |
| Plans | Create a plan, edit a plan, retrieve a plan, reset a plan, delete a plan | Public | plan_id | plan_id, ingredients, results |  |
| Buildings | Retrieve a building | Public | building_id | building_id, inputs, outputs, recipes, overclock_bool, clock_percent, power_usage, width, length, height, area, ingredients, category |  |
| Components | Retrieve a component | Public | component_id | component_id, stack_size, sink_value, recipes, ingredients, building_needed, category |  |
| Resources | Retrieve a resource | Public | resource_id | resource_id, stack_size, sink_value, node_type, building_needed, recipes |  |
| Calculate Output |  | Private | multiple inputs of building outputs | total_output |  |

Note: Double check Private VS Public endpoints to be sure these are correct.

## Backend Stack

Express - Restful API

JEST - Testing

MongoDB - Database

Mongoose - Modeling

## What is the MVP?

The MVP will contain a list of buildings, components and resources that will be calculated into how many items they produce. Nice to haves are an efficiency calculator to tell you how efficient your factory is, a visualization of what the factory could look like on a 1 tall by infinite long and wide plane and maybe a list of necessary items to make it happen.
