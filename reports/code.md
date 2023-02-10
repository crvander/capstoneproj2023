---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Code

### remove input, show output
<!-- remove input, show output -->
```{code-cell} ipython3
:tags: ["remove-input"]
python -m pip install pandas
import pandas as pd

df = pd.DataFrame({'name': ['carlos', 'diane'], 'gender': ['male', 'female']})
df
```


<script type="text/x-thebe-config">
  {
    binderOptions: {
      repo: "crvander/version",
      ref: "requirements_carlos",
    }
  }
</script>

<!-- Load the Thebe activation and status field library  !-->
<script src="{{ pathto('_static/thebe_status_field.js', 1) }}" type="text/javascript"></script>
<link rel="stylesheet" type="text/css" href="{{ pathto('_static/thebe_status_field.css', 1) }}"/>

<!-- Test whether some code cell contains Sage code
     If yes, setup the ThebeLab activation and status field !-->
<script>
  $(function() {
      var cellSelector = "pre:contains('sage: ')";
      if ($(cellSelector).length > 0) {
         $('<div class="thebe_status_field" style="position: fixed; right:0;"></div>')
            .prependTo('div.body');
         thebe_place_activate_button();
      }
  });
</script>



<!------------->




### Thebe
<!-- Configure and load Thebe !-->
<script type="text/x-thebe-config">
  {
      requestKernel: true,
      mountActivateWidget: true,
      mountStatusWidget: true,
      binderOptions: {
      repo: "binder-examples/requirements",
      },
  }
</script>

<script src="https://unpkg.com/thebe@latest/lib/index.js"></script>

<pre data-executable="true" data-language="python">print("Hello!")</pre>

<div class="thebe-activate"></div>
<div class="thebe-status"></div>


