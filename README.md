# 🥾 Bootcamp git avancé

## Plan

1. Présentation
2. Commandes de base
3. Merge et rebase
4. Cherry-pick
5. Rebase interactif
6. Push et Pull
7. Gestion des conflits
8. Configuration de git
9. Le reflog

## [Learn Git Branching](https://learngitbranching.js.org/)

 - [Rebase et merge feat1 dans main](https://learngitbranching.js.org/?NODEMO&command=importTreeNow%20%7B%22branches%22%3A%7B%22main%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C6%22%2C%22id%22%3A%22main%22%2C%22type%22%3A%22branch%22%7D%2C%22feat1%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C4%22%2C%22id%22%3A%22feat1%22%2C%22type%22%3A%22branch%22%7D%2C%22feat2%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C5%22%2C%22id%22%3A%22feat2%22%2C%22type%22%3A%22branch%22%7D%7D%2C%22commits%22%3A%7B%22C0%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Nov%2005%202012%2000%3A56%3A47%20GMT-0800%20%28PST%29%22%2C%22commitMessage%22%3A%22Quick%20Commit.%20Go%20Bears%21%22%2C%22id%22%3A%22C0%22%2C%22rootCommit%22%3Atrue%7D%2C%22C1%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C0%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Nov%2005%202012%2000%3A56%3A47%20GMT-0800%20%28PST%29%22%2C%22commitMessage%22%3A%22Quick%20Commit.%20Go%20Bears%21%22%2C%22id%22%3A%22C1%22%7D%2C%22C2%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C1%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A54%3A46%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C2%22%7D%2C%22C3%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A55%3A14%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C3%22%7D%2C%22C4%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C3%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A55%3A16%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C4%22%7D%2C%22C5%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A56%3A47%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C5%22%7D%2C%22C6%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%2C%22C5%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A57%3A10%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Merge%20de%20branch%20%5C%22feat2%5C%22%20dans%20branch%20%5C%22main%5C%22%22%2C%22id%22%3A%22C6%22%7D%7D%2C%22tags%22%3A%7B%7D%2C%22HEAD%22%3A%7B%22id%22%3A%22HEAD%22%2C%22target%22%3A%22feat1%22%2C%22type%22%3A%22general%20ref%22%7D%7D)
 - [Reporter C4 sur bar](https://learngitbranching.js.org/?NODEMO&command=importTreeNow%20%7B%22branches%22%3A%7B%22main%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C2%22%2C%22id%22%3A%22main%22%2C%22type%22%3A%22branch%22%7D%2C%22feat1-a%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C5%22%2C%22id%22%3A%22feat1-a%22%2C%22type%22%3A%22branch%22%7D%2C%22feat1-b%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C7%22%2C%22id%22%3A%22feat1-b%22%2C%22type%22%3A%22branch%22%7D%7D%2C%22commits%22%3A%7B%22C0%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Nov%2005%202012%2000%3A56%3A47%20GMT-0800%20%28PST%29%22%2C%22commitMessage%22%3A%22Quick%20Commit.%20Go%20Bears%21%22%2C%22id%22%3A%22C0%22%2C%22rootCommit%22%3Atrue%7D%2C%22C1%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C0%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Nov%2005%202012%2000%3A56%3A47%20GMT-0800%20%28PST%29%22%2C%22commitMessage%22%3A%22Quick%20Commit.%20Go%20Bears%21%22%2C%22id%22%3A%22C1%22%7D%2C%22C2%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C1%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A39%3A43%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C2%22%7D%2C%22C3%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A40%3A39%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C3%22%7D%2C%22C4%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C3%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A40%3A41%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C4%22%7D%2C%22C5%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C4%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A40%3A42%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C5%22%7D%2C%22C6%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A42%3A46%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C6%22%7D%2C%22C7%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C6%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A42%3A47%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C7%22%7D%7D%2C%22tags%22%3A%7B%7D%2C%22HEAD%22%3A%7B%22id%22%3A%22HEAD%22%2C%22target%22%3A%22feat1-a%22%2C%22type%22%3A%22general%20ref%22%7D%7D)
 - [Rebase feat2 sur main](https://learngitbranching.js.org/?NODEMO&command=importTreeNow%20%7B%22branches%22%3A%7B%22main%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C8%22%2C%22id%22%3A%22main%22%2C%22type%22%3A%22branch%22%7D%2C%22feat1%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C4%22%2C%22id%22%3A%22feat1%22%2C%22type%22%3A%22branch%22%7D%2C%22feat2%22%3A%7B%22remoteTrackingBranchID%22%3Anull%2C%22remote%22%3Afalse%2C%22target%22%3A%22C7%22%2C%22id%22%3A%22feat2%22%2C%22type%22%3A%22branch%22%7D%7D%2C%22commits%22%3A%7B%22C0%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A59%3A12%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C0%22%2C%22rootCommit%22%3Atrue%7D%2C%22C1%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C0%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2008%3A59%3A12%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C1%22%7D%2C%22C2%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C1%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A00%3A56%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C2%22%7D%2C%22C3%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A01%3A18%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C3%22%7D%2C%22C4%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C3%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A01%3A19%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C4%22%7D%2C%22C5%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C4%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A01%3A58%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C5%22%7D%2C%22C6%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C5%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A01%3A59%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C6%22%7D%2C%22C7%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C6%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A02%3A00%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C7%22%7D%2C%22C8%22%3A%7B%22type%22%3A%22commit%22%2C%22parents%22%3A%5B%22C2%22%5D%2C%22author%22%3A%22Peter%20Cottle%22%2C%22createTime%22%3A%22Mon%20Apr%2008%202024%2009%3A02%3A27%20GMT+0200%20%28Central%20European%20Summer%20Time%29%22%2C%22commitMessage%22%3A%22Commit%20rapide.%20NoMaN%20Sux%21%22%2C%22id%22%3A%22C8%22%7D%7D%2C%22tags%22%3A%7B%7D%2C%22HEAD%22%3A%7B%22id%22%3A%22HEAD%22%2C%22target%22%3A%22feat2%22%2C%22type%22%3A%22general%20ref%22%7D%7D)

## Configurer `git`

Documentation de [git-config](https://git-scm.com/docs/git-config).

### `push` et `pull` (et `fetch`)

#### [`push.autoSetupRemote`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-pushautoSetupRemote)

Pour éviter d'avoir à utiliser l'option `--set-upstream` ou `-u` de `git push` lors du tout 1er push d'une nouvelle branche:

```
git config --global push.autoSetupRemote true
```

#### [`pull.rebase`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-pullrebase)

Pour éviter d'avoir à utiliser l'option `--rebase` ou `-r` de `git pull`:

```
git config --global pull.rebase true
```

#### [`pull.ff`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-pullff)

Si vous ne souhaitez pas travailler en "pull rebase", vous pouvez interdire à `git pull` la création de commits de merge avec:

```
git config --global pull.ff only
```

Si le pull ne résulte pas en un *fast-forward*, alors rien ne se passe et un message d'erreur apparaît:

```
$ git pull
fatal: Not possible to fast-forward, aborting.
```

Ensuite à vous de gérer 😉

#### [`fetch.prune`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-fetchprune)

Pour éviter d'avoir à utiliser l'option `--prune` ou `-p` de `git pull` et `git fetch`:

```
git config --global fetch.prune true
```

Fait le ménage dans les branches distantes une fois que celles-ci n'existent plus sur le serveur:

```
$ git pull
 - [deleted]           (none)                                      -> origin/branche-mergee
```

> [!WARNING]
> Si vous avez travaillé sur `branche-mergee`, cela ne supprime pas votre branche locale.
> Pour supprimer la branche locale, il faut utiliser la commande `git branch -D branche-mergee`

### `rebase`

#### [`rebase.autoStash`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-rebaseautoStash)

Pour éviter d'avoir à utiliser l'option `--autostash` de `git rebase` et `git pull`:

```
git config --global rebase.autoStash true
```

Tout travail non commité sera rangé dans la remise avant un rebase, puis ressorti une fois le rebase terminé:

```
$ git rebase origin/dev
Created autostash: 2c587a8b
Applied autostash.
Successfully rebased and updated refs/heads/ma-branche.
```

> [!WARNING]
> Après un rebase réussi, des conflits peuvent être rencontrés lorsque le travail non commité est sorti de la remise.

#### [`rebase.autoSquash`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-rebaseautoSquash)

Pour éviter d'avoir à utiliser l'option `--autosquash` de `git rebase --interactive` ou `git rebase -i`:

```
git config --global rebase.autoSquash true
```

Lors du lancement d'un nouveau rebase interactif, les commits de squash et/ou de fixup créés précédemment seront automatiquement positionnés au bon endroit et avec la bonne commande dans le TODO généré.

#### [`rebase.updateRefs`](https://git-scm.com/docs/git-config#Documentation/git-config.txt-rebaseupdateRefs)

Pour éviter d'avoir à utiliser l'option `--update-refs` de `git rebase`:

```
git config --global rebase.updateRefs true
```

Dans le cas où:
 - `branche1` est basée sur `dev`
 - `branche2` est basée sur `branche1`

Alors si je souhaite mettre à jour `branche1` et `branche2` avec la dernière version de `dev`, je peux me positionner sur `branche2` et lancer un rebase:

```
$ git rebase dev
Successfully rebased and updated refs/heads/branche2.
Updated the following refs with --update-refs:
	refs/heads/branche1
```
