Copy and paste the following in the templates page of your HA to see all the entities and their attributes in one place in a well formatted way.

The information is formatted in such a way, that it can be used to customize, create groups and views to manage your entities.


START --------------------
The following are the entities that are recognized by the Home Assistant:
Just add components in the components list below for additional entities.

{%- set domains = [states.light, states.switch, states.automation, states.device_tracker, states.group, states.media_player, states.proximity, states.script, states.zone, states.zwave ] %}

{{ "Entity ID".ljust(50) }}  {{ "Entity Name" }}

{%- for domain in domains %}
{% for item in domain %}
{{ "_".ljust(90, "_") }}
{{ item.entity_id.ljust(50) }} {{ item.name }}
    State: {{ item.state}}
    Domain: {{ item.domain |title}}
    Object ID: {{ item.object_id }}
    Last Updated:  {{ item.last_updated }}
    Last Changed: {{ item.last_changed }}
    Icon: {{item.attributes.icon}}
    Supported Features: {{item.attributes.supported_features}}
    Brightness: {{item.attributes.brightness}}
    friendly_name: {{item.attributes.friendly_name}}
    color_temp: {{item.attributes.color_temp}}
    rgb_color: {{item.attributes.rgb_color}}
    unit_of_measurement: {{item.attributes.unit_of_measurement}}
    assumed_state: {{item.attributes.assumed_state}}
    entity_picture: {{item.attributes.entity_picture}}
    hidden: {{item.attributes.hidden}}
    last_triggered: {{item.attributes.last_triggered}}
{%- endfor %}
{%- endfor %}

END --------------------
