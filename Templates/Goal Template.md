<% '---' %>
noteType: goal
area: 
tags: goal
progress: 
target: 100
startDate: 
deadline: 
completionDate: 
completed: false
banner: https://images.unsplash.com/photo-1633158834806-766387547d2c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wzNjAwOTd8MHwxfHNlYXJjaHwxM3x8Z29hbHxlbnwwfDB8fHwxNzA4MTUzODc3fDA&ixlib=rb-4.0.3&q=80&w=1080
created_at: <% tp.file.creation_date('YYYY-MM-DD[T]HH:mm:ssZ') %>
<% '---' %>

>[!multi-column]
>
>>[!blank-container]
>>Start Date: `=this.startDate`
>
>>[!blank-container]
>>Deadline: `=this.deadline`
>
>>[!blank-container]
>>Compleione Date: `=this.completionDate`

<br>

>[!multi-column]
>
>>[!blank-container]
>>**Completed:** `INPUT[toggle:completed]` 
>
>>[!blank-container]
>>**Area:** `=this.area`

```meta-bind
INPUT[progressBar(title('Progress'), minValue(0), maxValue(100)):progress]
```

> [!info] Why is this goal important to me?
> 1. 

> [!success]- What would I gain by achieving this goal?
> 1. 

> [!failure]- What are the possible risks and obstacles?
> 1. 

## Sub Goals:


## Related:


<% await tp.file.move("/001 Goals/" + tp.file.title) %>