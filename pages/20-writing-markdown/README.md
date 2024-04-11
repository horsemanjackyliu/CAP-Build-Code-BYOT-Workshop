# Writing Markdown best practices

Markdown allows you to write engaging content, leverage the available formatting options, check this [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to see the possibilities. Additionally, Docsify allows us for a few more things.

## Images

To add an image, use the link:

```
![](link/to/the/image.jpg)
```

Assuming the image is in the folder `img/` at the same level than the markdown file:

```
![](./img/image.jpg)
```

## Link to files for download

> [!ATTENTION]
> Files to download should be in a folder called `files/`.

Assuming there is a `files/` folder in the same place as the markdown file

```
![](./files/document.pdf ':ignore :target=_self')
```

Note how the link always needs this part at the end:

```
':ignore :target=_self'
```


## Alerts and callouts

- Sample alert using type NOTE

```
> [!NOTE]
> An alert of type 'note' using global style 'callout'.
```

> [!NOTE]
> An alert of type 'note' using global style 'callout'.

- Sample alert using type TIP

```
> [!TIP]
> An alert of type 'tip' using global style 'callout'.
```

> [!TIP]
> An alert of type 'tip' using global style 'callout'.

- Sample alert using type WARNING

```
> [!WARNING]
> An alert of type 'warning' using global style 'callout'.
```

> [!WARNING]
> An alert of type 'warning' using global style 'callout'.

- Sample alert using type ATTENTION

```
> [!ATTENTION]
> An alert of type 'attention' using global style 'callout'.
```

> [!ATTENTION]
> An alert of type 'attention' using global style 'callout'.

- Sample alert for CONGRATULATIONS

```
> [!TIP|icon:fa-solid fa-check|label:Congratulations]
> You completed the exercise successfully.
```

> [!TIP|icon:fa-solid fa-check|label:Congratulations]
> You completed the exercise successfully.

## Emojis

You can directly copy and paste emojis in your pages 👍 (for example from [emojipedia.org](https://emojipedia.org)). If you need more options, you can also use icons from FontAwesome, search for an icon [in their website](https://fontawesome.com), copy the name, and write in in the format:

```
:name-of-icon:
```

For example:

```
:bell:
```

:bell:

## Tabs

You can create tabs to include options or variations in your exercises. See more info in [their page](https://jhildenbiddle.github.io/docsify-tabs/#/).

```
<!-- tabs:start -->

#### **English**

Hello!

#### **French**

Bonjour!

#### **Italian**

Ciao!

<!-- tabs:end -->
```

<!-- tabs:start -->

#### **English**

Hello!

#### **French**

Bonjour!

#### **Italian**

Ciao!

<!-- tabs:end -->