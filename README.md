<h3 align="center">
PPBench
</h3>
<p align="center">
PPBench:A benchmark for debugging PHP Python Languages
</p>

<p style="text-align: center">

[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
[![GitHub last commit](https://img.shields.io/github/last-commit/NoumanAhmad448/PPBench)](https://github.com/NoumanAhmad448/PPBench/commits/master)
[![GitHub contributors](https://img.shields.io/github/contributors/hiyouga/LLaMA-Factory?color=orange)](https://github.com/hiyouga/LLaMA-Factory/graphs/contributors)
[![GitHub workflow](https://github.com/hiyouga/LLaMA-Factory/actions/workflows/tests.yml/badge.svg)](https://github.com/hiyouga/LLaMA-Factory/actions/workflows/tests.yml)
[![PyPI](https://img.shields.io/pypi/v/llamafactory)](https://pypi.org/project/llamafactory/)
[![Citation](https://img.shields.io/badge/citation-238-green)](https://scholar.google.com/scholar?cites=12620864006390196564)
[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
</p>

## Table of Contents

- [Stackoverflow](#Stackoverflow)
- [Github](#github)
- [Kaggle](#kaggle)


## Stackoverflow
[Stackoverflow Chosen Tags List](/stackoverflow_unique_tags.json)

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

## Kaggle
[Kaggle Chosen Notebooks](/kaggle_urls.txt)

