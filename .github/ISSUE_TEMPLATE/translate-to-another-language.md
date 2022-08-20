---
name: Translate to another language
about: Propose your language version of the bot.
title: "[TRANSLATE]"
labels: enhancement, language
assignees: ''

---

⚠Replace only the text and not the lines of code to make it easier for me to insert ⚠

Language: 
<!--- Example: French --->

```js
// config command
// ...
                
                                     .setColor('#0099ff')
                                     .setTitle('Configuration')
                                     .setDescription('The configuration has been saved')
                                     .addField('Language', lang ? `\`${lang === "fr" ? "French" : "English"}\`` : 'None')
                                     .addField('Channel', notification ? `<#${notification}>` : 'None')
                                     .setTimestamp()
// ...
```

```js
// nookshop command
// ...

                                    .setTitle(`<:melimelo:998263104045596702> Offres de ${offer.name}`)
                                    .setURL(`https://turnip.exchange/island/${offer.turnipCode}`)
                                    .setColor('#0099ff')
                                    .setThumbnail('https://cdn.jsdelivr.net/npm/tapshort-add@1.0.6/tapservice/melimelo.png')
                                    .addFields(
{ name: '<:turnip:998231248415752322> Prix des navets', value: `${offer.turnipPrice} <:money:998231246989693058>`, inline: true }, 
{ name: '👫 File d\'attente', value: `\`${offer.queued}\``, inline: true }, 
{ name: ':coin: Pourboire', value: `${offer.fee ? "Oui": "Non"}`, inline: true }, 
{ name: '🌍 Hemisphere', value: `${offer.hemisphere === "north" ? "Nord" : "Sud"}`, inline: true }, 
{ name: '📆 Date', value: `\`${day + "/" + month + "/" + year + " à " + hourInt + ":" + minute }\``, inline: true }, 
{ name: ':star: Note', value: `${offer.rating ? offer.rating : "Aucune"} ⭐`, inline: true }
)
// ...

                                     .setTitle(`<:melimelo:998263104045596702> Offres du Nook Shop`)
                                    .setURL('https://turnip.exchange/islands/')
                                    .setThumbnail('https://cdn.jsdelivr.net/npm/tapshort-add@1.0.6/tapservice/melimelo.png')
                                    .setColor('#0099ff')
                                    .setDescription(`
                ${offers.slice(0, 5).map(offer => `
                **[${offer.name}](https://turnip.exchange/island/${offer.turnipCode})** \`${offer.turnipCode}\`
                - <:turnip:998231248415752322> Navet pour **${offer.turnipPrice} <:money:998231246989693058>** 
                - 👫 \`${offer.queued}\` 
                - :coin: Pourboire: **${offer.fee ? "Oui": "Non"}** `).join('\n')}`)
// ...
```

```js
// daisy command
// ...
                                    .setTitle(`<:daisy:998231245706231879> Offres de ${offer.name}`)
                                    .setURL(`https://turnip.exchange/island/${offer.turnipCode}`)
                                    .setColor('#0099ff')
                                    .setThumbnail('https://cdn.jsdelivr.net/npm/tapshort-add@1.0.6/tapservice/daisy.png')
                                    .addFields(
{ name: '<:turnip:998231248415752322> Prix des navets', value: `${offer.turnipPrice} <:money:998231246989693058>`, inline: true }, 
{ name: '👫 File d\'attente', value: `\`${offer.queued}\``, inline: true }, 
{ name: ':coin: Pourboire', value: `${offer.fee ? "Oui": "Non"}`, inline: true },
{ name: '🌍 Hemisphere', value: `${offer.hemisphere === "north" ? "Nord" : "Sud"}`, inline: true },
{ name: '📆 Date', value: `\`${day + "/" + month + "/" + year + " à " + hourInt + ":" + minute }\``, inline: true }, 
{ name: ':star: Note', value: `${offer.rating ? offer.rating : "Aucune"} ⭐`, inline: true })
// ...

                                    .setTitle(`<:daisy:998231245706231879> Offres de Daisy`)
                                    .setURL('https://turnip.exchange/islands/')
                                    .setColor('#0099ff')
                                    .setThumbnail('https://cdn.jsdelivr.net/npm/tapshort-add@1.0.6/tapservice/daisy.png')
                                    .setDescription(`
                ${offers.slice(0, 5).map(offer => `
                **[${offer.name}](https://turnip.exchange/island/${offer.turnipCode}) \`${offer.turnipCode}\`** 
                - <:turnip:998231248415752322> Navet pour **${offer.turnipPrice} <:money:998231246989693058>** 
                - 👫 \`${offer.queued}\` 
                - :coin: Pourboire: **${offer.fee ? "Oui": "Non"}** `).join('\n')}`)
//...
```

```js
// help command
//...
                .setColor('#fff562')
                .setTitle('Liste des commandes')
                .setDescription(commands.join('\n'))
                .setThumbnail('https://cdn.jsdelivr.net/npm/tapshort-add@1.0.8/tapservice/tom-nook.png')
//...
```
