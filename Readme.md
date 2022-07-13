# Mathpix

Forked from [oovm/Mathpix](https://github.com/oovm/Mathpix).

Use paclet manager to install the latest version:

```Mathematica
ResourceFunction["GitHubInstall"]["edisonlee55", "Mathpix"]
```

Apply for your API Key from https://dashboard.mathpix.com/signup, with one thousand free credits per month

Then set your key:

```Mathematica
PersistentValue["Mathpix", "Local"]={"$KeyName","$KeyValue"};
```

Load the function:

```Mathematica
Needs["Mathpix`"]
```

## Build

To build the paclet manually, first import the `PacletTools`:

```Mathematica
Needs["PacletTools`"]
```

Then build the paclet:

```Mathematica
PacletBuild["<path to the paclet source directory>"]
```

## Usage

Mathpix receives a `Image`, or the `String` of path to the image, or `MathpixAPI` object.

And have the following modes: `{N, D, E, Text, "Raw"}`.

## NormalMode

![Normal](https://i.loli.net/2018/12/01/5c0248400385c.png)

## DisplayMode

![Display](https://i.loli.net/2018/12/01/5c0248402b4b5.png)

## ExpressionMode

![Expression](https://i.loli.net/2018/12/01/5c02483fae878.png)

## RawMode

![Raw](https://i.loli.net/2018/12/01/5c024926664f1.png)