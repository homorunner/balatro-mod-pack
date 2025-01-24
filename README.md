# Awesome balatro mod pack

## Install

Install [Lovely](https://github.com/ethangreen-dev/lovely-injector) first.

After installing lovely, run following command in powershell:

```powershell
cd $env:APPDATA\Balatro

git clone --recursive https://github.com/homorunner/balatro-mod-pack.git

if (Test-Path -Path "Mods") {
    Get-ChildItem -Path "Mods" | ForEach-Object {
        Move-Item -Path $_.FullName -Destination "balatro-mod-pack" -ErrorAction Stop
    }
    Remove-Item -Path "Mods" -Recurse -Force -ErrorAction Stop
}

Rename-Item -Path "balatro-mod-pack" -NewName "Mods" -ErrorAction Stop
```

## FAQ

### Why scoring animation was lost?

Check Talisman settings, scoring animation is by default disabled in Talisman mod.

### I want FasterStakesUnlock mod.

FasterStakesUnlock is incompatible with Galdur. Use Galdur settings to unlock more stakes.

## Mods

### Aurinko

Author: jenwalter666

Github link: https://github.com/jenwalter666/JensBalatroCollection

Planet card can have editions.

### Betmma Voucher Pack

Author: Betmma, nicholassam6425, homorunner(localization)

Github link: https://github.com/betmma/my_balatro_mods

Adds 3 Voucher Packs.

### Cryptid

Author: MathIsFun_, Cryptid and Balatro Discords

Github link: https://github.com/MathIsFun0/Cryptid

A lot of cool new jokers, consumables, blinds and so on.

### Galdur

Author: Eremel

Github link: https://github.com/Eremel/Galdur

Improved startup screen.

### MoreFluff

Author: notmario

Github link: https://github.com/notmario/MoreFluff

Add a new consumable: Color card. Also adds some cool jokers.

### Talisman

Author: MathIsFun_, Mathguy24, jenwalter666, cg-223

Github link: https://github.com/MathIsFun0/Talisman

Increases the score cap, making it hard to reach nan/inf.

### Card Sleeves

Author: LarsWijn

Github link: https://github.com/larswijn/CardSleeves

Add card sleeves.

### Better Credit Card

Author: homorunner

Github link: https://github.com/homorunner/BetterCreditCard

Enhanced the original joker "Credit Card".

### Planet Card Cash Out

Author: antlers

Github link: https://github.com/antler5/Balatro-Planet-Card-Cash-Out-Mod

Allow using a planet card while the cash-out animation.

