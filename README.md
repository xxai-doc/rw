<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Birasabwa gushiraho nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) mbere, hanyuma `direnv allow` nyuma yo kwinjira mububiko ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) izakorwa mu buryo bwikora nyuma yo kwinjira mububiko).

Igisobanuro ni: Igishinwa cyahinduwe mu Kiyapani, Igikoreya, Icyongereza, Icyongereza mu zindi ndimi zose. Niba ushaka gushyigikira gusa igishinwa nicyongereza, urashobora kwandika `zh: en` .

Igisobanuro ni: Igishinwa cyahinduwe mu Kiyapani, Igikoreya, Icyongereza, Icyongereza mu zindi ndimi zose. Niba ushaka gushyigikira gusa igishinwa nicyongereza, urashobora kwandika `zh: en` .

* [kode y'imbere](https://github.com/xxai-art/web)
* [Ibipapuro byururimi kurubuga muri rusange](https://github.com/xxai-art/web/tree/main/i18n)
* [Urupapuro rwindimi zo kwinjira](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Urubuga Indimi nyinshi](https://github.com/xxai-doc)

Ururimi-rwambere rwo gutangiza porogaramu ni [@ w5 / ikawa_plus](http://npmjs.com/@w5/coffee_plus) , yongeraho ibintu bimwe na bimwe bishingiye ku nteruro ya coffeescript, reba [./Ikawa_plus.md](./coffee_plus.md) .

## Kuzamura imbuga za interineti ninyandiko

Wubake kumishinga 3 ikurikira

* [@ w5 / mdt](https://www.npmjs.com/package/@w5/mdt)

  Umugereka ni `.mdt` , urashobora gukoresha syntax isa na `<+ ./coffee_plus/import.js>` kugirango yerekane amadosiye yo hanze, hanyuma utange akamenyetso hamwe ninyongera `.md` .

* [@ w5 / trmd](https://www.npmjs.com/package/@w5/trmd)

  Ubusobanuro bwa Markdown ntabwo buzahindura code hamwe nu murongo, kandi bizabika interuro zahinduwe. Niba ibisobanuro byahinduwe ariko inyandiko yumwimerere ntabwo yahinduwe, kuyikora ntibizongera kwandika ibyahinduwe.

* [@ w5 / i18n](https://www.npmjs.com/package/@w5/i18n)

  Indimi zindimi zo guhindura `yaml` yakozwe kurubuga.

### Amabwiriza yo Guhindura Automatic Amabwiriza

Reba ububiko bwa code [xxai-art / doc](https://github.com/xxai-art/doc)

Birasabwa gushiraho nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) mbere, hanyuma `direnv allow` nyuma yo kwinjira mububiko ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) izakorwa mu buryo bwikora nyuma yo kwinjira mububiko).

Kugirango wirinde kode nini yasobanuwe mu ndimi amagana, nashizeho kode itandukanye kuri buri rurimi kandi nshinga umuryango wo kubika code base

Gushiraho ibidukikije bihinduka `GITHUB_ACCESS_TOKEN` hanyuma ukore [gukora.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) izahita ikora ububiko bwa code.

Birumvikana, urashobora kandi kubishyira muri code base.

Ubusobanuro bw'inyandiko yerekana [ibisobanuro.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Inyandiko yimyandikire isobanurwa gutya:

[bunx](https://bun.sh/docs/cli/bunx) ni umusimbura wa npx, byihuse. Birumvikana, niba udafite imigati yashizwemo, urashobora gukoresha `npx` aho.

`bunx mdt zh` ihindura `.mdt` mububiko bwa zh nka `.md` , reba dosiye 2 zahujwe hepfo

* [ikawa_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [ikawa_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` ni code yibanze yo gusobanura (niba ufite `nodejs` gusa, ariko `bun` na `direnv` ntabwo zashizweho, urashobora kandi gukoresha `npx i18n` kugirango uhindure).

Bizasobanura [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , iboneza rya `i18n.yml` muriyi nyandiko niyi ikurikira:

```
en:
zh: ja ko en
```

Igisobanuro ni: Igishinwa cyahinduwe mu Kiyapani, Igikoreya, Icyongereza, Icyongereza mu zindi ndimi zose. Niba ushaka gushyigikira gusa igishinwa nicyongereza, urashobora kwandika `zh: en` .

Iheruka ni [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , ikuramo ibiri hagati yumutwe wingenzi na subtitle ya mbere ya buri rurimi `README.md` kugirango itange ibyinjira `README.md` . Kode iroroshye cyane, urashobora kuyireba wenyine.

Google API ikoreshwa mugusemura kubuntu. Niba udashobora kugera kuri Google, nyamuneka shiraho kandi ushireho porokisi, nka:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Inyandiko yubusobanuro izatanga cache yahinduwe mububiko bwa `.i18n` , nyamuneka iyigenzure hamwe na `git status` hanyuma uyongere mububiko bwa code kugirango wirinde guhindurwa kenshi.

Nyamuneka koresha `bunx i18n` burigihe uhinduye ibisobanuro kugirango uhindure cache.

Niba inyandiko yumwimerere hamwe nubusobanuro byahinduwe icyarimwe, cache izitiranya, niba rero ushaka guhindura, urashobora guhindura imwe gusa, hanyuma ugakoresha `bunx i18n` kugirango uvugurure cache.
