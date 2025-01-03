# Project Setup Cont...

## Adding more files to the project

Here we add `NFT Images` & `NFT Metadata`.

The final project will have two folders:
`images` & `metadata`.

The `images` folder contains a bunch of _Crypto Punks_ `.png` files.
Grabbing them from this project is very helpful, so you don't have to create your own or find them elsewhere!

The `metadata` folder contains the `json` data for each `NFT`.
Here is an example of the first one:

```json
{
  "id": "175b3aba08e956c66a891c99b8cdcfe38a8dfb97",
  "name": "#1",
  "description": "A image of 1,000 generated punks",
  "image": "ipfs://QmQPEMsfd1tJnqYPbnTQCjoa8vczfsV1FmqZWgRdNQ7z3g/1.png",
  "edition": 1,
  "date": 1649379902184,
  "attributes": [
    {
      "trait_type": "Backgrounds",
      "value": "Coral"
    },
    {
      "trait_type": "Face",
      "value": "Body 6"
    },
    {
      "trait_type": "Hats and Hair",
      "value": "Mohawk"
    },
    {
      "trait_type": "Eyes and Glasses",
      "value": "Green Eyes"
    },
    {
      "trait_type": "Nose",
      "value": "Standard"
    },
    {
      "trait_type": "Mouth",
      "value": "Smile"
    }
  ]
}
```

Simply copy these two folders from the master zip into **your** project.

## Push to GitHub

Now would be a great time to push your project to `GitHub`.
First create a `repository on GitHub`.
Give the project a name that is unique and create.
`GitHub` will then give you some instructions for pushing your project up.

```bash
git add .
```

The `.` means you are pushing all files to `GitHub`.

```bash
git commit -m "initial commit"
```

Any message inside the `double quotes` will do. Very common for first commit to be `initial commit`.

```bash
git branch -M main
```

This will change the branch from `master` to `main`.
Not mandatory, but `GitHub` now really pushes for this and it is the new way to do things.

Next you will see a rather long command that is unique to your project.

```bash
git remote add origin https://github.com/username/projectname.git
```

Just copy/paste this line (from GitHub) into your terminal and hit `enter`.

Final step is to push to `GitHub`:

```bash
git push -u origin main
```

Because you added this `-u origin main`, you now will only need to use `git push` for every push going forward.
