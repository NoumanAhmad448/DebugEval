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
```
Technical Summary:
Avoid Duplication:

A check is added to verify if a notebook has already been processed by checking a processed_urls.txt file. If a URL is already in this file, it is skipped to prevent duplication.
Environment Variables:

All important paths and settings are moved to an .env file. The following variables are used:
URL_FILE: Path to the file containing notebook URLs.
OUTPUT_FILE: Path to store the JSONL output.
LOG_FILE: Path to store error logs.
DEBUG_LOG_FILE: Path to store debug logs.
PROCESSED_FILE: Path to store already processed URLs.
Logging:

logging module is used to log all actions.
Errors are logged in error.log.
Debug messages are logged in debug.log if the DEBUGGING flag is set to True.
Logs include details of every action performed: reading URLs, fetching comments, processing notebooks, and writing the output.
Duplication Check:

Each notebook URL is checked against the processed_urls.txt file before being processed.
If a notebook is already in the processed list, it is skipped, ensuring no duplication.
Processed URL Tracking:

After processing a notebook, its URL is written to processed_urls.txt to ensure it is not processed again in the future.
```
