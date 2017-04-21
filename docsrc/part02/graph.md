# graph

* see https://www.npmjs.com/package/gitbook-plugin-graph

## memo

* "graph"プラグインでWARNが出力されてGitBookが公開できないので見送り中
* 実行されなければWARNがでないのが難点


```
{% graph %}
    {
        "title":"cos(2*PI*x/2)*(1+0.5cos(2*PI*x/100))",     
        "grid":true,
        "xAxis": {
            "label":"Sample",
            "domain": [0,300]
        },
        "yAxis": {
            "label":"Amplitude",
            "domain": [-1.5,1.5]
        },
        "data": [
            { "fn": "cos(2*PI*x/2)*(1+0.5cos(2*PI*x/100))"},         
            { "fn": "(1+0.5cos(2*PI*x/100))"}
       ]
    }
{% endgraph %}
```
