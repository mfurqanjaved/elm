# 2021 Census Analysis

## 1. Occupation Distribution Across England and Wales

```json
{
  "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
  "description": "Distribution of occupations",
  "data": {
    "values": [{"occupation":"1. Managers, directors and senior officials","count":3547860},{"occupation":"2. Professional occupations","count":5606150},{"occupation":"3. Associate professional and technical occupations","count":3661036},{"occupation":"4. Administrative and secretarial occupations","count":2574696},{"occupation":"5. Skilled trades occupations","count":2849747},{"occupation":"6. Caring, leisure and other service occupations","count":2600177},{"occupation":"7. Sales and customer service occupations","count":2087093},{"occupation":"8. Process, plant and machine operatives","count":1940120},{"occupation":"9. Elementary occupations","count":2906835}]
  },
  "mark": {"type": "bar", "tooltip": true},
  "width": 600,
  "height": 400,
  "encoding": {
    "x": {
      "field": "occupation",
      "type": "nominal",
      "title": "Occupation",
      "axis": {"labelAngle": -45}
    },
    "y": {
      "field": "count",
      "type": "quantitative",
      "title": "Number of Workers"
    }
  }
}
```

## 2. Working Hours Distribution

```json
{
  "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
  "description": "Distribution of working hours",
  "data": {
    "values": [{"hours":"Full-time: 31 to 48 hours worked","count":16427670},{"hours":"Full-time: 49 or more hours worked","count":3065020},{"hours":"Part-time: 15 hours or less worked","count":2855094},{"hours":"Part-time: 16 to 30 hours worked","count":5425930}]
  },
  "mark": {"type": "arc", "tooltip": true},
  "width": 400,
  "height": 400,
  "encoding": {
    "theta": {"field": "count", "type": "quantitative"},
    "color": {
      "field": "hours",
      "type": "nominal",
      "title": "Working Hours"
    }
  }
}
```

## 3. Top 10 Regions by Workforce Size

```json
{
  "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
  "description": "Top 10 regions by workforce size",
  "data": {
    "values": [{"region":"Birmingham","count":442413},{"region":"Leeds","count":374065},{"region":"Buckinghamshire","count":273236},{"region":"Cornwall","count":254248},{"region":"Wiltshire","count":252348},{"region":"Sheffield","count":242007},{"region":"Bristol","count":238511},{"region":"Manchester","count":234286},{"region":"County Durham","count":222213},{"region":"Bradford","count":221138}]
  },
  "mark": {"type": "bar", "tooltip": true},
  "width": 600,
  "height": 400,
  "encoding": {
    "x": {
      "field": "region",
      "type": "nominal",
      "title": "Region",
      "axis": {"labelAngle": -45}
    },
    "y": {
      "field": "count",
      "type": "quantitative",
      "title": "Number of Workers"
    }
  }
}
```

## Analysis Insights

1. **Occupation Distribution Analysis:**
   The analysis of occupational distribution across England and Wales reveals significant insights into the workforce structure. Professional occupations clearly dominate the employment landscape with over 5.6 million workers, representing the largest employment category. This is followed by Associate professional and technical occupations with approximately 3.6 million workers. Notably, Process, plant and machine operatives form the smallest category with about 1.9 million workers. This distribution reflects a modern, service-oriented economy with a strong emphasis on professional and knowledge-based work. The high number of professionals suggests a workforce that is increasingly skilled and specialized, while the relatively lower numbers in traditional industrial occupations indicates the ongoing shift away from manufacturing-based employment.

2. **Working Hours Pattern Analysis:**
   The working hours distribution provides crucial insights into work patterns across the country. The data shows a clear predominance of full-time work (31-48 hours), with over 16.4 million workers falling into this category, representing the standard working pattern for most employees. There is also a substantial presence of part-time work (16-30 hours) with approximately 5.4 million workers, indicating significant workplace flexibility. Interestingly, the extreme ends of the spectrum - those working very short hours (15 or less) and very long hours (49 or more) - are less common but still significant, with about 2.9 million and 3.1 million workers respectively. This distribution suggests a labor market that accommodates diverse working patterns while maintaining traditional full-time employment as the norm.

3. **Regional Workforce Distribution Analysis:**
   The regional workforce distribution highlights significant geographical patterns in employment across England and Wales. Birmingham emerges as the leading employment hub with over 442,000 workers, followed by Leeds with approximately 374,000 workers. The dominance of major cities in the top positions, including Manchester, Sheffield, and Bristol, underscores the concentration of economic activity in urban centers. Interestingly, some non-metropolitan areas like Buckinghamshire and Cornwall also feature in the top 10, with workforces exceeding 250,000, suggesting significant economic activity outside the major cities. This pattern reflects both the traditional strength of urban employment centers and the emerging importance of regional economic hubs, painting a picture of a diverse and evolving economic geography.
