<h3 align="center">
PPBench
</h3>
<p align="center">
PPBench:A benchmark for debugging PHP Python Languages
</p>

<div align="center">

<a href="https://github.com/hiyouga/LLaMA-Factory/stargazers">
    <img src="https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social" alt="GitHub Repo stars"/>
</a>
<a href="https://github.com/NoumanAhmad448/PPBench/commits/master">
    <img src="https://img.shields.io/github/last-commit/NoumanAhmad448/PPBench" alt="GitHub last commit"/>
</a>
<a href="https://github.com/hiyouga/LLaMA-Factory/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/hiyouga/LLaMA-Factory?color=orange" alt="GitHub contributors"/>
</a>
<a href="https://github.com/hiyouga/LLaMA-Factory/actions/workflows/tests.yml">
    <img src="https://github.com/hiyouga/LLaMA-Factory/actions/workflows/tests.yml/badge.svg" alt="GitHub workflow"/>
</a>
<a href="https://pypi.org/project/llamafactory/">
    <img src="https://img.shields.io/pypi/v/llamafactory" alt="PyPI"/>
</a>
<a href="https://scholar.google.com/scholar?cites=12620864006390196564">
    <img src="https://img.shields.io/badge/citation-238-green" alt="Citation"/>
</a>
<a href="https://github.com/hiyouga/LLaMA-Factory/pulls">
    <img src="https://img.shields.io/badge/PRs-welcome-blue" alt="GitHub pull request"/>
</a>

</div>


## Table of Contents

- [Stackoverflow](#Stackoverflow)
- [Github](#github)


## Stackoverflow
[All Stackoverflow Chosen Tags List by using StackAPI Resource](/stackoverflow_unique_tags.json)
<br/>
[Stack API Link](https://api.stackexchange.com/docs/related-tags)

Basic List of Python list <br/>
```
NumPy, pandas, Matplotlib, Seaborn, SciPy, Scikit-learn, TensorFlow, Keras, PyTorch, Statsmodels, NLTK, SpaCy, Gensim, XGBoost, LightGBM, CatBoost, OpenCV, Pillow, Plotly, Bokeh, Dask, PySpark, NetworkX, Yellowbrick, Eli5, SHAP, Feature-engine, Imbalanced-learn, Pandas-profiling, Streamlit, Dash, FastAPI, SQLAlchemy, PyMySQL, Psycopg2, BeautifulSoup, Requests, Scrapy, PyOD, Prophet, PyCaret, Django, Flask, Theano, Caffe, MXNet, Numba, Cython, Joblib, Pickle.
```

Basic List of PHP
```
Laravel, Symfony, CodeIgniter, Zend Framework, Phalcon, Slim, Yii, CakePHP, Laminas, FuelPHP, Aura, PHPUnit, Guzzle, Monolog, PHP-DI, Twig, Blade, Doctrine, Eloquent, Propel, PHPExcel, PHPMailer, Swift Mailer, Faker, Carbon, PHP_CodeSniffer, PHPStan, Psalm, Composer, Packagist, PHPCS Fixer, PHP Mess Detector, PHPCPD, PHPBench, PHP_CompatInfo, PHP_CodeCoverage, PHP_Formatter, PHP_TokenStream, PHP_Reflection, PHP_Parser, PHP_CodeBrowser, PHP_Depend, PHP_ChangeLog, PHP_Documentor, PHP_UML, PHP_Beautifier, PHP_Compat, PHP_Console_Color, PHP_Console_Table, PHP_Console_ProgressBar
```
```
{
  "question_id": "39402823",
  "tags": ["c++", "algorithm", "opengl", "3d", "adjacency-matrix"],
  "instruction": "OpenGL triangle adjacency calculation",
  "input": "",
  "output": "<p>You are making it way more complicated than it needed to be. You want to search for triangles that share a specific edge and return the third vertex. Then just do so. </p>\n\n<pre><code>for(unsigned int i=0; i&lt;mesh.mNumFaces; ++i ) {\n    unsigned int*&amp; indices = mesh.mFaces[i].mIndices;\n    for(int edge = 0; edge &lt; 3; ++edge) { //iterate all edges of the face\n        unsigned int v1 = indices[edge]; //first edge index\n        unsigned int v2 = indices[(edge + 1) % 3]; //second edge index\n        unsigned int vOpp = indices[(edge + 2) % 3]; //index of opposite vertex\n        //if the edge matches the search edge and the opposite vertex does not match\n        if(((v1 == index1 &amp;&amp; v2 == index2) || (v2 == index1 &amp;&amp; v1 == index2)) &amp;&amp; vOpp != index3)\n            return vOpp; //we have found the adjacent vertex\n    }\n}\nreturn -1;\n</code></pre>\n\n<p>Furthermore, you need to change your calls. If you call the function three times with the same arguments, you will get the same results, of course:</p>\n\n<pre><code>index[1] = findAdjacentIndex( mesh, index[0], index[2], index[4] );\nindex[3] = findAdjacentIndex( mesh, index[2], index[4], index[0] );\nindex[5] = findAdjacentIndex( mesh, index[4], index[0], index[2] );\n</code></pre>\n",
  "system": ""
}
```

## Github
[Github chosen Repositories](/github_repos.json)
```
{
    "instruction": "BUG: array.ctypes.data_as is not memory safe",
    "output": "<p dir=\"auto\">This isn't a vulnerability at all, it is simply unsafe API.</p>",
    "input": "",
    "system": ""
},
```

