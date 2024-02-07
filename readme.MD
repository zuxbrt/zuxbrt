```php
<?php

namespace zuxbrt;

class About extends Me
{
    public function yearsOfExperience(): string
    {
        $started = new DateTime("2018-05-01");
        $today = new DateTime();
        $total = $started->diff($today);
        return $total->y;
    }

    public function getLocation(): array
    {
        return [
            'country' => 'Bosnia and Herzegovina',
            'city' => 'Sarajevo'         
        ];
    }

    public function getCurrentWorkplace(): array
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
        return 'to learn more and expand my stack';
    }
}
```

```javascript
const jsSkills = { 
  frameworksAndLibraries: "React", "NuxtJS", "ThreeJs", "EmberJs" 
  expandingKnowledgeAbout: "Typescript", "React"
}
```
