# MoveIt Serialization

Serializer for multiple ros messages including moveit_msgs. Supports yaml serialization through rapidyaml.

## Roadmap
- Add binary serealizer for ros_msgs

## rapidyaml
One of the fastest yaml parser and emiter available. <br>
Current version: https://github.com/captain-yoshi/rapidyaml/commit/e9ec9fcf5e6f34e5f44e48f1c1038cbb7e38b285

Configuration:
- Built internally to avoid unwanted changes to the global error handler.
- Custom `Tree::has_all` method for subset node comparaison (not yet merged).
- `C4_DEBUG_BREAK` is disabled at runtime in the error handler.

## Contribution
The conversion for decoding/encoding moveit_msgs in yaml-cpp was done by Zachary Kingston and taken from the [robowflex](https://github.com/KavrakiLab/robowflex) project.
