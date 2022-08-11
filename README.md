# Machine-Learning-Applications
This is a listing of machine learning tutorials, projects, and demos that were used as lessons at Clemson University. 

## Repositories
- [Discovery](https://github.com/efwoods/Discovery)
- [Holocaust Veterans](https://github.com/efwoods/Holocaust_Veterans)
- [Precision Agriculture](https://github.com/efwoods/Watson-Precision-Agriculture)
- [IBM Watson Assistant](https://github.com/efwoods/assistant-simple)
- [Car Dashboard](https://github.com/efwoods/car-dashboard)
- [IBM Watson Visual Recognition](https://github.com/efwoods/Watson-Visual-Recognition)


## Explaination
[Vue Mastery: BaseCheckbox](https://www.vuemastery.com/courses/vue3-forms/base-checkbox)

[BaseCheckbox.vue](./BaseCheckbox.vue)

- event structure (defined in App)
```
      event: {
        category: '',
        title: '',
        description: '',
        location: '',
        pets: 1,
        extras: {
          catering: false,
          music: false
        }
      }
```


```
<template>
  <input
    type="checkbox" // inputs with this type don't trigger @input events
    :checked="modelValue" // model is bound on checked property rather than value
    @change="$emit('update:modelValue', $event.target.checked)" 
      // change events are triggered (when using selected and onSelected)
      // $event.target.checked is the value of the checked status, ":checked"
    class="field"
  />
  <label v-if="label">{{ label }}</label>
</template>
```

## Prerequisites
None

## Use
```
        <BaseCheckbox
          v-model="event.extras.catering"
          label="Catering"
        />
```


[<BaseCheckbox v-model="event.extras.catering" label="Catering"/](https://gist.githubusercontent.com/efwoods/ea8d10c27ad2be109d75f607688fbe78/raw/a9af4127757421f9804e3ebc45a709a4f37af18d/BaseCheckbox.vue)
