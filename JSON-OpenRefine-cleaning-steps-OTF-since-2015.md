# Appendix G:JSON Code for otf_granting_data_since_april_1_2015 Data cleanup in [OpenRefine](https://openrefine.org/)

All 48 data updates!

```JSON
[
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Geographical Area Served:Région servis",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Waterloo, Wellington, Dufferin",
          "Waterloo, Wellington & Dufferin"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Waterloo, Wellington, Dufferin"
      }
    ],
    "description": "Mass edit cells in column Geographical Area Served:Région servis"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Organization name:Nom d'organisme",
    "expression": "value",
    "edits": [
      {
        "from": [
          "FarmStart",
          "Farmstart"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "FarmStart"
      },
      {
        "from": [
          "Community Innovation Lab",
          "community innovation lab"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Community Innovation Lab"
      }
    ],
    "description": "Mass edit cells in column Organization name:Nom d'organisme"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Program Area:Région de programme",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Prosperous People",
          "Prosperous people"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Prosperous People"
      }
    ],
    "description": "Mass edit cells in column Program Area:Région de programme"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.trim()",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.trim()"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(/\\s+/,' ')",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(/\\s+/,' ')"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\"Ontario\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\"Ontario\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(/\\bCorp\\b/,\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(/\\bCorp\\b/,\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\"Corporation\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\"Corporation\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\"#\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\"#\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(/number/i,\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(/number/i,\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\"(\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\"(\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\")\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\")\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\",\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\",\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(/\\bProv\\b/,\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(/\\bProv\\b/,\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\"BN\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\"BN\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.replace(\"ON\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.replace(\"ON\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value.trim()",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation using expression value.trim()"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Municipality",
          "municipality"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Municipality"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [
        {
          "type": "list",
          "name": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
          "expression": "value",
          "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
          "invert": false,
          "omitBlank": false,
          "omitError": false,
          "selection": [
            {
              "v": {
                "v": "338776",
                "l": "338776"
              }
            },
            {
              "v": {
                "v": "0338776",
                "l": "0338776"
              }
            }
          ],
          "selectBlank": false,
          "selectError": false
        }
      ],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value",
    "edits": [
      {
        "from": [
          "0338776",
          "338776"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "0338776"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation",
    "expression": "value",
    "edits": [
      {
        "from": [
          "1009062",
          "10090602"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "1009062"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Incorporation Number:Org du bénéficiaires: Numéro d'incorporation"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:City:Org du bénéficiaires:Ville",
    "expression": "value.trim()",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:City:Org du bénéficiaires:Ville using expression value.trim()"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(/\\s+/,' ')",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(/\\s+/,' ')"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"-\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"-\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"#\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"#\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "grel:value.replace(\"BN\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression grel:value.replace(\"BN\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\":\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\":\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\".\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\".\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"rr\",\"RR\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"rr\",\"RR\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"• Canada Revenue Agency Registration\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"• Canada Revenue Agency Registration\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"(incorporatedJune27,1956)\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"(incorporatedJune27,1956)\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"(incorporated June 27, 1956)\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"(incorporated June 27, 1956)\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"Letters Patent 253788\",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"Letters Patent 253788\",\"\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RR001\",\"RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RR001\",\"RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RC\",\"RR\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RC\",\"RR\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RT\",\"RR\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RT\",\"RR\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RP\",\"RR\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RP\",\"RR\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"r\",\"R\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"r\",\"R\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RRR\",\"RR\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RRR\",\"RR\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RR001\",\"RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RR001\",\"RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"000RR\",\"RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"000RR\",\"RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RR00014\",\"RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RR00014\",\"RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"107761694 RR 0194\",\"107761694RR0028\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"107761694 RR 0194\",\"107761694RR0028\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"11930 3782 RR 0001 1951\",\"119303782RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"11930 3782 RR 0001 1951\",\"119303782RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.replace(\"RR 0001\",\"RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.replace(\"RR 0001\",\"RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "grel:value.replace(\" RR0001\",\"RR0001\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression grel:value.replace(\" RR0001\",\"RR0001\")"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value.trim()",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression value.trim()"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "grel:value.replace(\" \",\"\")",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance using expression grel:value.replace(\" \",\"\")"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance",
    "expression": "value",
    "edits": [
      {
        "from": [
          "113412114RR0001",
          "133412114RR0001"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "113412114RR0001"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Charitable Registration Number: Org du bénéficiaires:Numéro d'enregistrement d'organisme de bienfaisance"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:City:Org du bénéficiaires:Ville",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Toronto",
          "TORONTO",
          "toronto",
          "Toronto,"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Toronto"
      },
      {
        "from": [
          "Kingston",
          "KINGSTON",
          "Kingston,",
          "kingston"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Kingston"
      },
      {
        "from": [
          "St. Catharines",
          "St Catharines",
          "ST CATHARINES"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "St. Catharines"
      },
      {
        "from": [
          "Chatham",
          "CHATHAM",
          "chatham"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Chatham"
      },
      {
        "from": [
          "Barrie",
          "BARRIE",
          "barrie"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Barrie"
      },
      {
        "from": [
          "Orléans",
          "ORLEANS",
          "ORLÉANS"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Orléans"
      },
      {
        "from": [
          "Oshawa",
          "OSHAWA",
          "oshawa"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Oshawa"
      },
      {
        "from": [
          "Leamington",
          "LEAMINGTON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Leamington"
      },
      {
        "from": [
          "Richmond Hill",
          "Richmond  Hill"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Richmond Hill"
      },
      {
        "from": [
          "Lansdowne",
          "LANSDOWNE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Lansdowne"
      },
      {
        "from": [
          "RESTOULE",
          "Restoule"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Restoule"
      },
      {
        "from": [
          "OHSWEKEN",
          "Ohsweken"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Ohsweken"
      },
      {
        "from": [
          "Kitchener",
          "KITCHENER"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Kitchener"
      },
      {
        "from": [
          "London",
          "LONDON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "London"
      },
      {
        "from": [
          "Almonte",
          "ALMONTE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Almonte"
      },
      {
        "from": [
          "Sault Ste. Marie",
          "SAULT STE MARIE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Sault Ste. Marie"
      },
      {
        "from": [
          "SMOOTH ROCK FALLS",
          "Smooth Rock Falls"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Smooth Rock Falls"
      },
      {
        "from": [
          "Guelph",
          "GUELPH"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Guelph"
      },
      {
        "from": [
          "St. Thomas",
          "ST. THOMAS"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "St. Thomas"
      },
      {
        "from": [
          "Windsor",
          "WINDSOR"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Windsor"
      },
      {
        "from": [
          "WINNIPEG",
          "Winnipeg"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Winnipeg"
      },
      {
        "from": [
          "Bobcaygeon",
          "BOBCAYGEON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Bobcaygeon"
      },
      {
        "from": [
          "Mount Brydges",
          "MOUNT BRYDGES"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Mount Brydges"
      },
      {
        "from": [
          "Oakville",
          "OAKVILLE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Oakville"
      },
      {
        "from": [
          "Essex",
          "ESSEX"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Essex"
      },
      {
        "from": [
          "North Bay",
          "NORTH BAY"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "North Bay"
      },
      {
        "from": [
          "Opasatika",
          "OPASATIKA"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Opasatika"
      },
      {
        "from": [
          "Ottawa",
          "OTTAWA"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Ottawa"
      },
      {
        "from": [
          "Niagara On The Lake",
          "NIAGARA ON THE LAKE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Niagara On The Lake"
      },
      {
        "from": [
          "Hamilton",
          "HAMILTON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Hamilton"
      },
      {
        "from": [
          "Lindsay",
          "LINDSAY"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Lindsay"
      },
      {
        "from": [
          "Thornhill",
          "THORNHILL"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Thornhill"
      },
      {
        "from": [
          "Markdale",
          "MARKDALE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Markdale"
      },
      {
        "from": [
          "Scarborough",
          "SCARBOROUGH"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Scarborough"
      },
      {
        "from": [
          "Bracebridge",
          "BRACEBRIDGE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Bracebridge"
      },
      {
        "from": [
          "ECHO BAY",
          "Echo Bay"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Echo Bay"
      },
      {
        "from": [
          "Cornwall",
          "CORNWALL"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Cornwall"
      },
      {
        "from": [
          "Georgetown",
          "georgetown"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Georgetown"
      },
      {
        "from": [
          "Whitby",
          "WHITBY"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Whitby"
      },
      {
        "from": [
          "Burlington",
          "BURLINGTON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Burlington"
      },
      {
        "from": [
          "Mississauga",
          "MISSISSAUGA"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Mississauga"
      },
      {
        "from": [
          "Newmarket",
          "NEWMARKET"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Newmarket"
      },
      {
        "from": [
          "Ajax",
          "AJAX"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Ajax"
      },
      {
        "from": [
          "Orillia",
          "ORILLIA"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Orillia"
      },
      {
        "from": [
          "Woodbridge",
          "WOODBRIDGE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Woodbridge"
      },
      {
        "from": [
          "Sarnia",
          "SARNIA"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Sarnia"
      },
      {
        "from": [
          "Sutton West",
          "SUTTON WEST"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Sutton West"
      },
      {
        "from": [
          "Picton",
          "picton"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Picton"
      },
      {
        "from": [
          "Carleton Place",
          "CARLETON PLACE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Carleton Place"
      },
      {
        "from": [
          "Midland",
          "MIDLAND"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Midland"
      },
      {
        "from": [
          "DESBARATS",
          "Desbarats"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Desbarats"
      },
      {
        "from": [
          "Etobicoke",
          "Etobicoke,"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Etobicoke"
      },
      {
        "from": [
          "Brampton",
          "BRAMPTON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Brampton"
      },
      {
        "from": [
          "Aurora",
          "AURORA"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Aurora"
      },
      {
        "from": [
          "Brockville",
          "BROCKVILLE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Brockville"
      },
      {
        "from": [
          "GRIMSBY",
          "Grimsby"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Grimsby"
      },
      {
        "from": [
          "Peterborough",
          "PETERBOROUGH"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Peterborough"
      },
      {
        "from": [
          "Welland",
          "WELLAND"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Welland"
      },
      {
        "from": [
          "Sudbury",
          "SUDBURY"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Sudbury"
      },
      {
        "from": [
          "Lanark",
          "LANARK"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Lanark"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:City:Org du bénéficiaires:Ville"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:City:Org du bénéficiaires:Ville",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Mississauga",
          "Misssissauga"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Mississauga"
      },
      {
        "from": [
          "St. Catharines",
          "St. Cathariines"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "St. Catharines"
      },
      {
        "from": [
          "St. Catharines",
          "St.Catharines"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "St. Catharines"
      },
      {
        "from": [
          "Douro Dummer",
          "Douro Drummer"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Douro Dummer"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:City:Org du bénéficiaires:Ville"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:City:Org du bénéficiaires:Ville",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Sault Ste. Marie",
          "SAULT STE-MARIE"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Sault Ste. Marie"
      },
      {
        "from": [
          "Niagara On The Lake",
          "Niagara-on-the-Lake"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Niagara On The Lake"
      },
      {
        "from": [
          "Mississauga",
          "Missississauga"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Mississauga"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:City:Org du bénéficiaires:Ville"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:City:Org du bénéficiaires:Ville",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Cambridge",
          "Cambridge, ON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Cambridge"
      },
      {
        "from": [
          "Kingston",
          "Kingston ON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Kingston"
      },
      {
        "from": [
          "Penetanguishene",
          "Penetanguishene ON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Penetanguishene"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:City:Org du bénéficiaires:Ville"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:City:Org du bénéficiaires:Ville",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Toronto",
          "Toronto ON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Toronto"
      },
      {
        "from": [
          "Tyendinaga Mohawk Territory",
          "Tyendinaga Territory"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Tyendinaga Mohawk Territory"
      },
      {
        "from": [
          "Ottawa",
          "Ottawa ON"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Ottawa"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:City:Org du bénéficiaires:Ville"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0N1H0",
          "p0n1h0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0N1H0"
      },
      {
        "from": [
          "K1K 1G8",
          "K1K 1G8 "
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1K 1G8"
      },
      {
        "from": [
          "M5V3A8",
          " M5V3A8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V3A8"
      },
      {
        "from": [
          "L9M 2G3",
          "L9m 2G3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9M 2G3"
      },
      {
        "from": [
          "N0L 2P0",
          "N0L 2P0 "
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0L 2P0"
      },
      {
        "from": [
          "N1R-8E3",
          "N1R8E3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1R 8E3"
      },
      {
        "from": [
          "K0H2P0",
          "k0h2P0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0H 2P0"
      },
      {
        "from": [
          "K0L 1L0",
          "K0l 1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0l 1L0"
      },
      {
        "from": [
          "M5G1Z8 ",
          "M5G1Z8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5G 1Z8 "
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P7C 3N9",
          "P7C3N9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P7C 3N9"
      },
      {
        "from": [
          "N2G 1V6",
          "N2G1V6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 1V6"
      },
      {
        "from": [
          "K0J 1T0",
          "K0J1T0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0J 1T0"
      },
      {
        "from": [
          "K0M 2K0",
          "K0M-2K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0M 2K0"
      },
      {
        "from": [
          "K0L 1C0",
          "K0L1C0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0L 1C0"
      },
      {
        "from": [
          "N0J 1G0",
          "N0J1G0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0J 1G0"
      },
      {
        "from": [
          "V6B 6E3",
          "V6B6E3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "V6B 6E3"
      },
      {
        "from": [
          "M5A 1T3",
          "M5A1T3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 1T3"
      },
      {
        "from": [
          "N6L 1E3",
          "N6L1E3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6L 1E3"
      },
      {
        "from": [
          "K1K 2C7",
          "K1K2C7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1K 2C7"
      },
      {
        "from": [
          "N4K2H7",
          "N4K 2H7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4K 2H7"
      },
      {
        "from": [
          "K7L 4T9",
          "K7L4T9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7L 4T9"
      },
      {
        "from": [
          "M5J 2G8",
          "M5J2G8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5J 2G8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0T2J0",
          "P0T 2J0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0T 2J0"
      },
      {
        "from": [
          "P7B 1C4",
          "P7B1C4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P7B 1C4"
      },
      {
        "from": [
          "M4L 3M2",
          "M4L3M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4L 3M2"
      },
      {
        "from": [
          "L8K 5P5",
          "L8K5P5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8K 5P5"
      },
      {
        "from": [
          "L4R 4K6",
          "L4R4K6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4R 4K6"
      },
      {
        "from": [
          "N5Y 4K4",
          "N5Y4K4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5Y 4K4"
      },
      {
        "from": [
          "M5R 1X3",
          "m5r1x3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5R 1X3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9T 0H8",
          "L9T0H8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9T 0H8"
      },
      {
        "from": [
          "N0M1L0",
          "N0M 1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0M 1L0"
      },
      {
        "from": [
          "M3J 2P3",
          "M3J2P3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3J 2P3"
      },
      {
        "from": [
          "N9B 2E9",
          "N9B2E9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9B 2E9"
      },
      {
        "from": [
          "P6A 2G4",
          "P6A2G4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A 2G4"
      },
      {
        "from": [
          "L6T 3T6",
          "L6T3T6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6T 3T6"
      },
      {
        "from": [
          "K0M 1A0",
          "K0M1A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0M 1A0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6P4A9",
          "M6P 4A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6P 4A9"
      },
      {
        "from": [
          "K1S 3E2",
          "K1S3E2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1S 3E2"
      },
      {
        "from": [
          "M2R 1W6",
          "M2R1W6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2R 1W6"
      },
      {
        "from": [
          "L4M 2Y1",
          "L4M2Y1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4M 2Y1"
      },
      {
        "from": [
          "N0G 1P0",
          "N0G1P0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0G 1P0"
      },
      {
        "from": [
          "N6B 2N8",
          "N6B2N8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6B 2N8"
      },
      {
        "from": [
          "L2V 4Y6",
          "L2V-4Y6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2V 4Y6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0R 1E0",
          "P0R1E0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0R 1E0"
      },
      {
        "from": [
          "L5B3C9",
          "L5B 3C9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5B 3C9"
      },
      {
        "from": [
          "N6H 1A5",
          "N6H1A5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6H 1A5"
      },
      {
        "from": [
          "N8X4M5",
          "N8X 4M5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N8X 4M5"
      },
      {
        "from": [
          "M6A 2T9",
          "M6A2T9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6A 2T9"
      },
      {
        "from": [
          "P3E 1C5",
          "P3E1C5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3E 1C5"
      },
      {
        "from": [
          "N6A 1C9",
          "N6A1C9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6A 1C9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2H 2G9",
          "N2H2G9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2H 2G9"
      },
      {
        "from": [
          "K1S 5B4",
          "K1S5B4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1S 5B4"
      },
      {
        "from": [
          "N6G 1G5",
          "N6G1G5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6G 1G5"
      },
      {
        "from": [
          "L0M 1T0",
          "L0M1T0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0M 1T0"
      },
      {
        "from": [
          "L2E 7H3",
          "L2E7H3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2E 7H3"
      },
      {
        "from": [
          "M3C3N6",
          "M3C 3N6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3C 3N6"
      },
      {
        "from": [
          "L6V 1N9",
          "L6V1N9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6V 1N9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9Y 4E8",
          "L9Y4E8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9Y 4E8"
      },
      {
        "from": [
          "L8N 3Y3",
          "L8N3Y3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8N 3Y3"
      },
      {
        "from": [
          "M3C 3A1",
          "M3C3A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3C 3A1"
      },
      {
        "from": [
          "M4J 1L2",
          "M4J1L2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4J 1L2"
      },
      {
        "from": [
          "L8P 4N7",
          "L8P4N7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8P 4N7"
      },
      {
        "from": [
          "N3Y 4L2",
          "N3Y4L2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3Y 4L2"
      },
      {
        "from": [
          "N0L 2P0",
          "N0L2P0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0L 2P0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2H3N3",
          "L2H 3N3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2H 3N3"
      },
      {
        "from": [
          "M4R1K8",
          "M4R 1K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4R 1K8"
      },
      {
        "from": [
          "N5Z 3L1",
          "N5Z3L1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5Z 3L1"
      },
      {
        "from": [
          "M6E 2H4",
          "M6E2H4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6E 2H4"
      },
      {
        "from": [
          "L3B 3X1",
          "L3B3X1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3B 3X1"
      },
      {
        "from": [
          "N0A 1M0",
          "N0A1M0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0A 1M0"
      },
      {
        "from": [
          "K1S 1C4",
          "K1S1C4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1S 1C4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5A 3A3",
          "M5A3A3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 3A3"
      },
      {
        "from": [
          "N7S 1H8",
          "N7S1H8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7S 1H8"
      },
      {
        "from": [
          "M6K 3P6",
          "M6K3P6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6K 3P6"
      },
      {
        "from": [
          "K1C1J4",
          "K1C 1J4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1C 1J4"
      },
      {
        "from": [
          "L6T 5E2",
          "L6T5E2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6T 5E2"
      },
      {
        "from": [
          "M5S 2R4",
          "M5S2R4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5S 2R4"
      },
      {
        "from": [
          "K7K 3E1",
          "K7K3E1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7K 3E1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N8X 1K7",
          "N8X1K7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N8X 1K7"
      },
      {
        "from": [
          "M5A 2G2",
          "M5A2G2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 2G2"
      },
      {
        "from": [
          "K4M 1A4",
          "K4M1A4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K4M 1A4"
      },
      {
        "from": [
          "K1S 5R5",
          "K1S5R5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1S 5R5"
      },
      {
        "from": [
          "L0S 1T0",
          "L0S1T0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0S 1T0"
      },
      {
        "from": [
          "M4H 1N7",
          "M4H1N7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4H 1N7"
      },
      {
        "from": [
          "M5T 2C2",
          "M5T2C2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5T 2C2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N6H 3E5",
          "N6H3E5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6H 3E5"
      },
      {
        "from": [
          "K0C1A0",
          "K0C 1A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0C 1A0"
      },
      {
        "from": [
          "L3R 1N1",
          "L3R1N1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3R 1N1"
      },
      {
        "from": [
          "M5R 2S7",
          "M5R2S7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5R 2S7"
      },
      {
        "from": [
          "N0C1H0",
          "N0C 1H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0C 1H0"
      },
      {
        "from": [
          "P0J 1K0",
          "P0J1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0J 1K0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1S 2L3",
          "K1S2L3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1S 2L3"
      },
      {
        "from": [
          "M6M3W3",
          "M6M 3W3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6M 3W3"
      },
      {
        "from": [
          "K1Z 6V1",
          "K1Z6V1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1Z 6V1"
      },
      {
        "from": [
          "K1K 2Z8",
          "K1K2Z8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1K 2Z8"
      },
      {
        "from": [
          "P0S 1C0",
          "P0S1C0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0S 1C0"
      },
      {
        "from": [
          "L4M 4T2",
          "L4M4T2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4M 4T2"
      },
      {
        "from": [
          "L4R 5N6",
          "L4R5N6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4R 5N6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5B 2P3",
          "M5B2P3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5B 2P3"
      },
      {
        "from": [
          "L0E 1R0",
          "L0E1R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0E 1R0"
      },
      {
        "from": [
          "K9J 3H1",
          "K9J3H1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9J 3H1"
      },
      {
        "from": [
          "K1N 6E2",
          "K1N6E2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 6E2"
      },
      {
        "from": [
          "L2E 6S5",
          "L2E6S5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2E 6S5"
      },
      {
        "from": [
          "L7P 1B7",
          "L7P1B7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L7P 1B7"
      },
      {
        "from": [
          "M6K 3C5",
          "M6K3C5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6K 3C5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0B 1S0",
          "N0B1S0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0B 1S0"
      },
      {
        "from": [
          "M5V 3C1",
          "M5v3c1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 3C1"
      },
      {
        "from": [
          "L6A 2A2",
          "L6A2A2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6A 2A2"
      },
      {
        "from": [
          "N9A4N1",
          "N9A 4N1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 4N1"
      },
      {
        "from": [
          "K0J 2A0",
          "K0J2A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0J 2A0"
      },
      {
        "from": [
          "K9H 7E7",
          "K9H7E7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 7E7"
      },
      {
        "from": [
          "N2B 2B4",
          "N2B2B4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2B 2B4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L7R 3M4",
          "L7R3M4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L7R 3M4"
      },
      {
        "from": [
          "N3S 3N2",
          "N3S3N2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3S 3N2"
      },
      {
        "from": [
          "L4A 7G4",
          "L4A7G4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4A 7G4"
      },
      {
        "from": [
          "M5V 3A8",
          "M5V3A8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 3A8"
      },
      {
        "from": [
          "L4T 3W4",
          "L4T3W4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4T 3W4"
      },
      {
        "from": [
          "M6A 3B4",
          "M6A3B4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6A 3B4"
      },
      {
        "from": [
          "P9A 3P9",
          "P9A3P9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P9A 3P9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0L 2H0",
          "K0L2H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0L 2H0"
      },
      {
        "from": [
          "N7M 3R5",
          "N7M3R5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7M 3R5"
      },
      {
        "from": [
          "K0A1A0",
          "K0A 1A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0A 1A0"
      },
      {
        "from": [
          "K0K 1H0",
          "K0K1H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 1H0"
      },
      {
        "from": [
          "N1R 7A5",
          "N1R7A5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1R 7A5"
      },
      {
        "from": [
          "L4N 6S7",
          "L4N6S7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4N 6S7"
      },
      {
        "from": [
          "N3R 4J8",
          "N3R4J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3R 4J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4R 1A1",
          "M4R1A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4R 1A1"
      },
      {
        "from": [
          "M4G3E8",
          "M4G 3E8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4G 3E8"
      },
      {
        "from": [
          "N6A1G3",
          "N6A 1G3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6A 1G3"
      },
      {
        "from": [
          "M9A 1B2",
          "M9A1B2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M9A 1B2"
      },
      {
        "from": [
          "K1E 3J4",
          "K1E3J4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1E 3J4"
      },
      {
        "from": [
          "M4R 1B1",
          "M4R1B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4R 1B1"
      },
      {
        "from": [
          "L7R4M4",
          "L7R 4M4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L7R 4M4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3Y 7B7",
          "L3Y7B7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 7B7"
      },
      {
        "from": [
          "N2G 4N5",
          "N2G4N5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 4N5"
      },
      {
        "from": [
          "K1Y1P4",
          "K1Y 1P4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1Y 1P4"
      },
      {
        "from": [
          "N0H 2R0",
          "N0H2R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0H 2R0"
      },
      {
        "from": [
          "L3Y 1K5",
          "L3Y1K5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 1K5"
      },
      {
        "from": [
          "M8V 2Z6",
          "M8V2Z6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M8V 2Z6"
      },
      {
        "from": [
          "M8V 2Z5",
          "M8V2Z5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M8V 2Z5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M9B 6E6",
          "M9B6E6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M9B 6E6"
      },
      {
        "from": [
          "M5A 2B7",
          "M5A2B7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 2B7"
      },
      {
        "from": [
          "L3X 1Z9",
          "L3X1Z9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3X 1Z9"
      },
      {
        "from": [
          "M5V 3B1",
          "M5V3B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 3B1"
      },
      {
        "from": [
          "K0K 2T0",
          "K0K2T0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 2T0"
      },
      {
        "from": [
          "L2T 4C2",
          "L2T4C2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2T 4C2"
      },
      {
        "from": [
          "K8N 2S6",
          "K8N2S6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K8N 2S6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2H 2M2",
          "N2H2M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2H 2M2"
      },
      {
        "from": [
          "M6C 2M1",
          "M6C2M1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6C 2M1"
      },
      {
        "from": [
          "L0E 1E0",
          "L0E1E0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0E 1E0"
      },
      {
        "from": [
          "M5S1X7",
          "M5S 1X7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5S 1X7"
      },
      {
        "from": [
          "K0H 2Y0",
          "K0H2Y0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0H 2Y0"
      },
      {
        "from": [
          "L2R3C7",
          "L2R 3C7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 3C7"
      },
      {
        "from": [
          "L2E 2L4",
          "L2E2L4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2E 2L4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4W 3X8",
          "M4W3X8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4W 3X8"
      },
      {
        "from": [
          "K0L 3C0",
          "K0L3C0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0L 3C0"
      },
      {
        "from": [
          "L6W 1T7",
          "L6W1T7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6W 1T7"
      },
      {
        "from": [
          "L4R 1R2",
          "L4R1R2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4R 1R2"
      },
      {
        "from": [
          "M6H 1K9",
          "M6H1K9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6H 1K9"
      },
      {
        "from": [
          "P0H 1Z0",
          "p0h1z0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0H 1Z0"
      },
      {
        "from": [
          "K2P 1X3",
          "K2P1X3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2P 1X3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1Y 4X5",
          "K1Y4X5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1Y 4X5"
      },
      {
        "from": [
          "M4P2H4",
          "M4P 2H4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4P 2H4"
      },
      {
        "from": [
          "N5C6A9",
          "N5C 6A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5C 6A9"
      },
      {
        "from": [
          "N3T 1E1",
          "N3T1E1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3T 1E1"
      },
      {
        "from": [
          "L1H 1W8",
          "L1H1W8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1H 1W8"
      },
      {
        "from": [
          "P0T 2A0",
          "P0T2A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0T 2A0"
      },
      {
        "from": [
          "L5N 1M2",
          "L5N1M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5N 1M2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N5Z 1E6",
          "N5Z1E6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5Z 1E6"
      },
      {
        "from": [
          "N9A 4N2",
          "N9A4N2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 4N2"
      },
      {
        "from": [
          "K0l 1L0",
          "K0L1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0l 1L0"
      },
      {
        "from": [
          "K1K 1N1",
          "K1K1N1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1K 1N1"
      },
      {
        "from": [
          "L6H 6M8",
          "L6H6M8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6H 6M8"
      },
      {
        "from": [
          "M5C1J3",
          "M5C 1J3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5C 1J3"
      },
      {
        "from": [
          "L2A 5M4",
          "L2A5M4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2A 5M4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0P 1H0",
          "P0P1H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0P 1H0"
      },
      {
        "from": [
          "N9E 4r9",
          "N9E4r9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9E 4R9"
      },
      {
        "from": [
          "N6B 1K8",
          "N6B1K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6B 1K8"
      },
      {
        "from": [
          "L0B 1B0",
          "L0B1B0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0B 1B0"
      },
      {
        "from": [
          "L6L 5M2",
          "L6L5M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6L 5M2"
      },
      {
        "from": [
          "P0P 1K0",
          "P0P1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0P 1K0"
      },
      {
        "from": [
          "L6Y 4M3",
          "L6Y4M3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6Y 4M3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P2N 3P4",
          "P2N3P4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P2N 3P4"
      },
      {
        "from": [
          "N0L 1W0",
          "N0L1W0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0L 1W0"
      },
      {
        "from": [
          "P0V 2M0",
          "P0V2M0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0V 2M0"
      },
      {
        "from": [
          "K1N 8Z6",
          "K1N8Z6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 8Z6"
      },
      {
        "from": [
          "K1K 1G8",
          "K1K1G8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1K 1G8"
      },
      {
        "from": [
          "K8V 3X4",
          "K8V3X4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K8V 3X4"
      },
      {
        "from": [
          "M5H 3S6",
          "M5H3S6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5H 3S6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6L 6R4",
          "L6L6R4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6L 6R4"
      },
      {
        "from": [
          "P1L 1S4",
          "P1L1S4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1L 1S4"
      },
      {
        "from": [
          "N5A 2M4",
          "N5A2M4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5A 2M4"
      },
      {
        "from": [
          "K0G 1K0",
          "K0G1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0G 1K0"
      },
      {
        "from": [
          "N6E 2H6",
          "N6E2H6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6E 2H6"
      },
      {
        "from": [
          "M6N 1K9",
          "M6N1K9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6N 1K9"
      },
      {
        "from": [
          "L8P 4Y3",
          "L8P4Y3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8P 4Y3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2S 0B4",
          "L2S0B4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2S 0B4"
      },
      {
        "from": [
          "K9J 2N4",
          "K9J2N4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9J 2N4"
      },
      {
        "from": [
          "M6J 1E3",
          "M6J1E3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6J 1E3"
      },
      {
        "from": [
          "M5B 1J3",
          "M5B1J3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5B 1J3"
      },
      {
        "from": [
          "P1B 1A8",
          "P1B1A8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1B 1A8"
      },
      {
        "from": [
          "K0E 1L0",
          "K0E1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0E 1L0"
      },
      {
        "from": [
          "N3W 2N9",
          "N3W2N9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3W 2N9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4J 2P5",
          "L4J2P5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4J 2P5"
      },
      {
        "from": [
          "L9Y 3Z1",
          "L9Y3Z1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9Y 3Z1"
      },
      {
        "from": [
          "M5T 2C7",
          "M5T2C7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5T 2C7"
      },
      {
        "from": [
          " N0M 1K0",
          "N0M1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0M 1K0"
      },
      {
        "from": [
          "L3B 3L2",
          "L3B3L2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3B 3L2"
      },
      {
        "from": [
          "K1G 4J8",
          "K1G4J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1G 4J8"
      },
      {
        "from": [
          "M4W 3L4",
          "M4W3L4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4W 3L4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4B 1L9",
          "L4B1L9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4B 1L9"
      },
      {
        "from": [
          "P0M 1K0",
          "P0M1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0M 1K0"
      },
      {
        "from": [
          "P3C 5E1",
          "P3C5E1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3C 5E1"
      },
      {
        "from": [
          "K9H 3V8",
          "K9H3V8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 3V8"
      },
      {
        "from": [
          "K9H3V1",
          "K9H 3V1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 3V1"
      },
      {
        "from": [
          "L3Y 4V9",
          "L3Y4V9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 4V9"
      },
      {
        "from": [
          "N3Y 5B3",
          "N3Y5B3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3Y 5B3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0M 1S0",
          "K0M1S0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0M 1S0"
      },
      {
        "from": [
          "N0P 1A0",
          "N0P1A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0P 1A0"
      },
      {
        "from": [
          "K1H7X3",
          "K1H 7X3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1H 7X3"
      },
      {
        "from": [
          "N0B 2J0",
          "N0B2J0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0B 2J0"
      },
      {
        "from": [
          "N9A 4C4",
          "N9A4C4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 4C4"
      },
      {
        "from": [
          "P0L 1N0",
          "P0L1N0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0L 1N0"
      },
      {
        "from": [
          "M5A 3C4",
          "M5A3C4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 3C4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0S 1J0",
          "L0S1J0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0S 1J0"
      },
      {
        "from": [
          "N1H 6J2",
          "N1H6J2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1H 6J2"
      },
      {
        "from": [
          "K1L 6P5",
          "K1L6P5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1L 6P5"
      },
      {
        "from": [
          "K7L 2X4",
          "K7L2X4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7L 2X4"
      },
      {
        "from": [
          "L2R 3K8",
          "L2R3K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 3K8"
      },
      {
        "from": [
          "N6A5P6",
          "N6A 5P6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6A 5P6"
      },
      {
        "from": [
          "L3Y 2A7",
          "L3Y2A7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 2A7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4S 2C6",
          "M4S2C6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4S 2C6"
      },
      {
        "from": [
          "K0K 1M0",
          "K0K1M0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 1M0"
      },
      {
        "from": [
          "K8A 6Y6",
          "K8A6Y6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K8A 6Y6"
      },
      {
        "from": [
          "K9H 2H7",
          "K9H2H7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 2H7"
      },
      {
        "from": [
          "P1B 1G5",
          "P1B1G5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1B 1G5"
      },
      {
        "from": [
          "L3Y 2N1",
          "L3Y2N1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 2N1"
      },
      {
        "from": [
          "K1L7L5",
          "K1L 7L5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1L 7L5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          ", ON M4K 2Y6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4K 2Y6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/text-transform",
    "engineConfig": {
      "facets": [
        {
          "type": "list",
          "name": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
          "expression": "value",
          "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
          "invert": false,
          "omitBlank": false,
          "omitError": false,
          "selection": [
            {
              "v": {
                "v": "M4K 2Y6",
                "l": "M4K 2Y6"
              }
            }
          ],
          "selectBlank": false,
          "selectError": false
        }
      ],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value.trim()",
    "onError": "keep-original",
    "repeat": false,
    "repeatCount": 10,
    "description": "Text transform on cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale using expression value.trim()"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          " L8V 1M1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8V 1M1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          " M6G 3B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6G 3B1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          " N2Z 2X6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2Z 2X6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          " N7A 1M6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7A 1M6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0B1R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0B 1R0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0E1X0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0E 1X0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0H1T0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0H 1T0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0C1G0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0C 1G0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0G1G0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0G 1G0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0J1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0J 1L0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "k0j1y0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "KOJ 1YO"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0J2R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0J 2R0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0K2K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 2K0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0K1C0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 1C0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0K1E0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 1E0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0K3K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0K 3K0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1G5Z6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1G 5Z6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1G4M3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1G 4M3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1G0B7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1G 0B7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0M1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0M 1K0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0M1N0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0M 1N0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0M2B0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0M 2B0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1N5M8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 5M8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1N5M9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 5M9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1N5S7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 5S7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1N7L7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 7L7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1N8P4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1N 8P4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1P1B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1P 1B1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1T0G6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1T 0G6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1T3W6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1T 3W6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1V1A8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1V 1A8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1V9W7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1V 9W7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1B3P5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1B 3P5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2A 1R9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2A 1R9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2A0S9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2A 0S9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2a1W5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2A 1W5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1Y0H3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1Y 0H3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0J2N0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0J 2N0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1L8H2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1L 8H2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1L7X5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1L 7X5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2B7Y4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2B 7Y4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2E7K1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2E 7K1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2E8A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2E 8A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2H5E4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2H 5E4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2H6N2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2H 6N2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2P0J9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2P 0J9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2P0T6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2P 0T6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2P1A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2P 1A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K2P1B7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K2P 1B7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K4B1N1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K4B 1N1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K6H7P6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K6H 7P6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K6J4K9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K6J 4K9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K6V5V2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K6V 5V2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K6V6J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K6V 6J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "k7h 1b7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7H 1B7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K7L5J7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7L 5J7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9H1W7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 1W7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9H2P4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 2P4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9H4C7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 4C7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9H7P9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9H 7P9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9J3H8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9J 3H8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9J5K4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9J 5K4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9V0J5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9V 0J5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9V3L9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9V 3L9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9V3LS"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9V 3LS"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0g1a0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0G 1A0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0L 1Xo"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0L 1X0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0L1T0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0L 1T0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0L2E5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0L 2E5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1H1A3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1H 1A3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1H4G1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1H 4G1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1H4G8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1H 4G8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1J8N5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1J 8N5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1K1E9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1K 1E9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2R2P8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 2P8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2R2Z3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R2Z3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2R2Z3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 2Z3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2R3M3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 3M3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2R4V9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 4V9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2R7R9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2R 7R9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2S4A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2S 4A1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3K4V1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3K 4V1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3M0A3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3M 0A3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3R8C1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3R 8C1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3S2J2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3S 2J2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3T2C6 "
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3T 2C6 "
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3T5W4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3T 5W4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3V1T4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3V 1T4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3V5B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3V 5B1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3X1K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3X 1K8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3X3E3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3X 3E3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3Y1X5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 1X5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3Y3W3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3Y 3W3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4G1L8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4G 1L8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4G3V5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4G 3V5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4G1N8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4G 1N8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4G5L6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4G 5L6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4J3M8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4J 3M8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4J8G6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4J 8G6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4J9J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4J 9J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4L0A2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4L 0A2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4M3M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4M 3M2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4M5R4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4M 5R4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4N2P7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4N 2P7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4N7Y9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4N 7Y9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4N9R3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4N 9R3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4R2R4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4R 2R4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4W4B6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4W 4B6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L4Y2N5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L4Y 2N5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5B2N5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5B 2N5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5B2N6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5B 2N6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5B3B9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5B 3B9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5B4B8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5B 4B8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5C2K6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5C 2K6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5E2J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5E 2J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5H1E9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5H 1E9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5K2P3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5K 2P3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5L4X9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5L 4X9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5N1A4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5N 1A4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5N7K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5N 7K8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L5T2E2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L5T 2E2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6A0T3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6A 0T3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6J0A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6J 0A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6J7W1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6J 7W1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6K2H2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6K 2H2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6K3C6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6K 3C6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6K5R2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6K 5R2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6M2Y1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6M 2Y1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6X5A5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6X 5A5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L7G5X8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L7G 5X8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L7N3N1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L7N 3N1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L7L5M4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L7L 5M4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8H3Y7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8H 3Y7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8L4N5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8L 4N5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8L5W8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8L 5W8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8N1B2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8N 1B2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8N2Z1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8N 2Z1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8P3C1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8P 3C1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8R1B9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8R 1B9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8S1L4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8S 1L4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9B2L6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9B 2L6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9C1C5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9C 1C5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9G2A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9G 2A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9H1X8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9H 1X8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9T8R2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9T 8R2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9T2Y3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9T 2Y3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9W1K1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9W 1K1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9W2Y8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9W 2Y8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9Y3Z5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9Y 3Z5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1E1W7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1E 1W7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1G3M5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1G 3M5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1H2W1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1H 2W1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1N1T3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1N 1T3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1V5E6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1V 5E6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1V5L3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1V 5L3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M2H1J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2H 1J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M2M4G8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2M 4G8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M2N5W9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2N 5W9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M2N6K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2N 6K8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M2R3V2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2R 3V2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M2R3V3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M2R 3V3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3A1A3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3A 1A3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3B3H9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3B. 3H9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3B. 3H9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3B 3H9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3N1W7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3N 1W7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3N2K4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3N 2K4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3J3H9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3J 3H9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3N3A6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3N 3A6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4A1E6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4A 1E6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4B2E2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4B 2E2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4C1L7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4C 1L7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4G1Z4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4G 1Z4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4J1M9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4J 1M9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4K1A2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4K 1A2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4L1G7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4L 1G7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4L1S6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4L 1S6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4M1G9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4M 1G9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4M3G3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4M 3G3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4M3P3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4M 3P3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4N2M1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4N 2M1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4P1G8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4P 1G8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4P2E5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4P 2E5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4S1C5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4S 1C5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4Y1B5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4Y 1B5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4Y1m1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4Y 1M1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5A2A8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 2A8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5A2V2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 2V2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5A2V8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 2V8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5A4C9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5A 4C9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5C1P1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5C 1P1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5C2C5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5C 2C5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5G1K2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5G 1K2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5G1L7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5G 1L7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5G1S5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5G 1S5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5G1P4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5G 1P4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5H3Y4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5H 3Y4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5J2H1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5J 2H1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5J2L6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5J 2L6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5R3H8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5R 3H8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5S2C7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5S 2C7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5S2T9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5S 2T9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5T2N8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5T 2N8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5T2Z5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5T 2Z5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5V1B5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 1B5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5V2L4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 2L4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5V2W7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 2W7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M5V1R9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M5V 1R9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6E2X1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6E 2X1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6G3L6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6G 3L6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6H1A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6H 1A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6H1M3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6H 1M3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6H1M9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6H 1M9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6H3J2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6H 3J2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6H3L9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6H 3L9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6J0A2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6J 0A2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6J1C5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6J 1C5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6N2Z1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6N 2Z1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6N3H1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6N 3H1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6P1Y8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6P 1Y8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6M4R3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6M 4R3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6P3K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6P 3K8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6P3Z5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6P 3Z5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6R2L8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6R 2L8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6R3B5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6R 3B5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M8W1B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M8W 1B1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M8W2B2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M8W 2B2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "m8z1k2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M8Z 1K2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0A1N0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0A 1N0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0B1P0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0B 1P0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0E1R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0E 1R0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0E1Y0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0E 1Y0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0G-2E0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0G 2E0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0G1B0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0G 1B0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0G2H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0G 2H0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0G2M0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0G 2M0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0G2N0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0G 2N0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0H1A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0H 1A0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0K1V0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0K 1V0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0K1Z0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0K 1Z0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0L1J0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0L 1J0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0P1R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0P 1R0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0N1R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0N 1R0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0R1A0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0R 1A0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N0R1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N0R 1K0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N1G2W1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1G 2W1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N1H8E8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1H 8E8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N1M2L4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1M 2L4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N1R8J5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1R 8J5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N1R8P2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N1R 8P2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2B0A2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2B 0A2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2C2H6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2C 2H6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2C2L9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2C 2L9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2E3Y4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2E 3Y4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2G1A3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 1A3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2G2E9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 2E9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2G2L3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 2L3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2G3V2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 3V2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2G4Y9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2G 4Y9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N2J2G9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N2J 2G9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3A2K6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3A 2K6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "n3b3m4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3B 3M4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3B1E1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3B 1E1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3C2A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3C 2A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3L3E1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3L 3E1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3H4R8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3H 4R8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "n3R 4y2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3R 4Y2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3T2X1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3T 2X1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3T5G9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3T 5G9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N3Y3R9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N3Y 3R9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4B1Z9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4B 1Z9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4G0C4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4G 0C4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4K5R1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4K 5R1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4L1A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4L 1A1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4N1R9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4N 1R9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4S6X5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4S 6X5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4W1L3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4W 1L3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4X1B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4X 1B1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N4X1B6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N4X 1B6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N5H1R5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5H 1R5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N5P1B7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5P 1B7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N5R3W9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5R 3W9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N5R5V1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N5R 5V1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N6A3C7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6A 3C7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N6B2J9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6B 2J9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N6C1A7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6C 1A7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N6C6A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N6C 6A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N7A1R6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7A 1R6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N7G1K9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7G 1K9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N7M5K4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7M 5K4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N7T2Z1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7T 2Z1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N7T7H8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7T 7H8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N7T7X2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N7T 7X2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N8H3W3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N8H 3W3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9A1W2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 1W2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9A3K8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 3K8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9A4N7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 4N7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9A5X3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9A 5X3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9C1A7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9C 1A7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9G1A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9G 1A1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N9H1S4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N9H 1S4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0A1X0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0A 1X0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0A1Z0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0A 1Z0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0H1E0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0H 1E0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0L1H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0L 1H0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0M1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0M 1L0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0M2G0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0M 2G0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0N1H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0N 1H0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0S1K0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0S 1K0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0T1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0T 1L0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0T2S0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0T 2S0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0V1X0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0V 1X0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "p0x 1p0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0X 1P0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0X1J0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0X 1J0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P1B4A6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1B 4A6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P1L1V4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1L 1V4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P1L1Z6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1L 1Z6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P1H1N9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P1H 1N9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P2A2W9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P2A 2W9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P2A2X4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P2A 2X4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P2B1T1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P2B 1T1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3A6A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3A 6A1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3A6B1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3A 6B1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3C1X5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3C 1X5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3C4X8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3C 4X8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3E0B2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3E 0B2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3E2X7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3E 2X7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P3E4S4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P3E 4S4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P4N-1K1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P4N 1K1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P5N2C8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P5N 2C8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6A1Z4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A 1Z4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6A1Z8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A. 1Z8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6A. 1Z8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A 1Z8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6A2A4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A 2A4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6A2E5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A 2E5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6A2T5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6A 2T5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P6B4J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P6B 4J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P7B1H3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P7B 1H3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P7B6J4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P7B 6J4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P7C3J6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P7C 3J6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P9A3M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P9A 3M2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P9N3x3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P9N 3X3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "POR1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "POR 1L0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "R3B0T4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "R3B 0T4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "T2H2A7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "T2H 2A7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "V8P3S1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "V8P 3S1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K0H1V0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K0H 1V0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K1C7C6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K1C 7C6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K7C2V8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7C 2V8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K7C3P3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7C 3P3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K7H1S9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7H 1S9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K7K3C1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7K 3C1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K7M4X4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K7M 4X4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K8N1G1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K8N 1G1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K8N4Z5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K8N 4Z5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K8P3P1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K8P 3P1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9A3B2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9A 3B2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9J6X5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9J 6X5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "K9J7H6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "K9J 7H6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0C1H0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0C 1H0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L0S1B0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L0S 1B0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1N6A9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1N 6A9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1N9B2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1N 9B2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1W3G7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1W 3G7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1S1M7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1S 1M7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1W4C2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1W 4C2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1Y1A1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1Y 1A1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1S1R6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1S 1R6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L1C5M2"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L1C 5M2"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2M4Y7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2M 4Y7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2M6T3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2M 6T3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2N1L5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2N 1L5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L2N6P8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L2N 6P8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3B3W7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3B 3W7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3B5R4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3B 5R4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L3B6A4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L3B 6A4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L6M3L1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L6M 3L1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L8V1 A8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L8V 1A8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9R1V1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9R 1V1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9R1W1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9R 1W1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9S1L0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9S 1L0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "L9W1V5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "L9W 1V5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M1S1T4"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M1S 1T4"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M3C1Y8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3C 1Y8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "m3c2c3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3C 2C3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "m3c2j6"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M3C 2J6"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4T2T5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4T 2T5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4Y1M7"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4Y 1M7"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4Y1V3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4Y 1V3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4Y2T7 "
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4Y 2T7 "
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M4Y2W5"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M4Y 2W5"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6A1C3"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6A 1C3"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6J2J8"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6J 2J8"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6K1X9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6K 1X9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "m6k1y9"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6K 1Y9"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "M6K3C1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "M6K 3C1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "N8M2Y1"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "N8M 2Y1"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Recipient Org:Postal Code: Org du bénéficiaires:code postale",
    "expression": "value",
    "edits": [
      {
        "from": [
          "P0L1R0"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "P0L 1R0"
      }
    ],
    "description": "Mass edit cells in column Recipient Org:Postal Code: Org du bénéficiaires:code postale"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Population Served:Population servis",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Diverse Cultural Communities and Racialized Groups",
          "Diverse Cultural Communities"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Diverse Cultural Communities and Racialized Groups"
      },
      {
        "from": [
          "LGBTTQIA",
          "LGBTTQ+"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "LGBTTQIA"
      }
    ],
    "description": "Mass edit cells in column Population Served:Population servis"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Population Served:Population servis",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Indigenous or Aboriginal",
          "Indigenous"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Indigenous or Aboriginal"
      }
    ],
    "description": "Mass edit cells in column Population Served:Population servis"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Population Served:Population servis",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Aboriginal"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Indigenous or Aboriginal"
      }
    ],
    "description": "Mass edit cells in column Population Served:Population servis"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Seniors (+65)",
          "Seniors (65+)"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Seniors (65+)"
      }
    ],
    "description": "Mass edit cells in column Age Group:Groupe d'âge"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Adults (25-64)",
          "Adults"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Adults (25-64)"
      },
      {
        "from": [
          "General population (all age groups)",
          "General Populations"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "General population (all age groups)"
      },
      {
        "from": [
          "Seniors (65+)",
          "Seniors"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Seniors (65+)"
      }
    ],
    "description": "Mass edit cells in column Age Group:Groupe d'âge"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Children"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Children up to 12 years"
      }
    ],
    "description": "Mass edit cells in column Age Group:Groupe d'âge"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Adults; Seniors (65+)"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Adults (25-64); Seniors (65+)"
      }
    ],
    "description": "Mass edit cells in column Age Group:Groupe d'âge"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Adults (25-64); Seniors (65+)"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Adults (25-64);Seniors (65+)"
      }
    ],
    "description": "Mass edit cells in column Age Group:Groupe d'âge"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Youth; Seniors (65+)"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Youth;Seniors (65+)"
      }
    ],
    "description": "Mass edit cells in column Age Group:Groupe d'âge"
  },
  {
    "op": "core/column-split",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Age Group:Groupe d'âge",
    "guessCellType": true,
    "removeOriginalColumn": true,
    "mode": "separator",
    "separator": ";",
    "regex": false,
    "maxColumns": 2,
    "description": "Split column Age Group:Groupe d'âge by separator"
  },
  {
    "op": "core/mass-edit",
    "engineConfig": {
      "facets": [],
      "mode": "row-based"
    },
    "columnName": "Grant Result:Résultat de subvention",
    "expression": "value",
    "edits": [
      {
        "from": [
          "Programs are safe, inclusive, and fair;",
          "Programs are safe, inclusive, and fair"
        ],
        "fromBlank": false,
        "fromError": false,
        "to": "Programs are safe, inclusive, and fair"
      }
    ],
    "description": "Mass edit cells in column Grant Result:Résultat de subvention"
  },
  {
    "op": "core/column-removal",
    "columnName": "Column",
    "description": "Remove column Column"
  }
]
```
