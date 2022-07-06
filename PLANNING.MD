# Satisfactory Planner

## API

| Endpoint            | Functionality                                                                           | Public or Private | Parameters   | Returns                                                                                                                               | Notes |
| ------------------- | --------------------------------------------------------------------------------------- | ----------------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Users               | Create a user, edit a user, retrieve a user, reset a password, view profile, view plans | Public            |              |                                                                                                                                       |       |
| Plans               | Create a plan, edit a plan, retrieve a plan, reset a plan, delete a plan                | Public            |              |                                                                                                                                       |       |
| Buildings           | Retrieve a building                                                                     | Public            | building_id  | building_id, inputs, outputs, recipes, overclock_bool, clock_percent, power_usage, width, length, height, area, ingredients, category |       |
| Components          | Retrieve a component                                                                    | Public            | component_id | component_id, stack_size, sink_value, recipes, ingredients, building_needed, category                                                 |       |
| Resources           | Retrieve a resource                                                                     | Public            | resource_id  | resource_id, stack_size, sink_value, node_type, building_needed, recipes                                                              |       |
| Calculate Output    |                                                                                         | Private           |              |                                                                                                                                       |       |
| Calculate Resources |                                                                                         | Private           |              |                                                                                                                                       |       |

Note: Double check Private VS Public endpoints to be sure these are correct.

## OBJECTS

**BUILDING**

**COMPONENT**

- Stack Size
- Sink Value
- Related Recipes
- Resources Needed
- Building Needed
- Items Produced Per Minute
- Clock Speed Percentage

**RESOURCE**

- Stack Size
- Sink Value
- Node Type (Pure, Normal, Impure)
- Items Produced Per Minute
- Clock Speed Percentage
- Related Recipes
- Building Needed
