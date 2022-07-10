# Pipes in angular
Pipes transform values in the html templates
## Built in pipes 

Examples 

`{{ title | uppercase }}`
`{{ today | date: 'dd/MM/yyyy' }}`

## Custom pipes

Create a class and implement PipeTransform from angular core.

```
    transform(value: any, ...args: any[]) {

        return value.substring(0,10);
       
    }
```
You should then add the Classname in app.module.ts in the declarations section.

In the pipe class add the annotation to name your pipe 

```
@Pipe({
    'name': 'shorten'
})
```







