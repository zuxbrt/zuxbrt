```php
<?php

namespace zuxbrt;

class About extends Me
{
    public function yearsOfExperience(): integer
    {
        $started = new DateTime("2018-05-01");
        $today = new DateTime();
        $total = $started->diff($today);
        return $total->y;
    }

    public function basedIn(): array
    {
        return [
            'country' => 'Bosnia and Herzegovina',
            'city' => 'Sarajevo'         
        ];
    }

    public function currentlyWorkingAt(): array
    {
        return [
            'company' => 'Purplekey',
            'position' => 'Full Stack Developer'         
        ];
    }

    public function getBackendStack(): array
    {
        return [
            PHP::class,
            Laravel::class,
            MySQL::class,
            Ubuntu::class
        ];
    }

    public function goals(): string
    {
        return 'learn more and expand my knowledge and my current stack';
    }
}
```

```javascript
const jsSkills = { 
  frameworksToolsAndLibraries: "React", "NuxtJS", "VueJs", "ThreeJs", "EmberJs", "Node"
  expandingKnowledgeAbout: "Typescript", "React"
}
```
