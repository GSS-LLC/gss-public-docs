# GSS Public Documentation

## დანიშნულება

ეს არის GSS პროდუქტების ერთიანი, საჯარო ცოდნის ბაზა. მისი მიზანია მომხმარებელმა - ბუღალტერმა, მენეჯერმა, ადმინისტრატორმა ან მხარდაჭერის თანამშრომელმა - კოდის, შიდა სისტემების ან ტექნიკური გუნდის ჩართვის გარეშე შეძლოს პროდუქტის ფუნქციის გაგება და ყოველდღიურ საქმეში გამოყენება.

აქ იწერება:

- რას აკეთებს პროდუქტი და რომელი სამუშაო ამოცანისთვის გამოიყენება;
- როგორ გამოიყენოს მომხმარებელმა ეკრანები, ველები, ფილტრები და ძებნა;
- რეალური, ადამიანურად წასაკითხი მაგალითები და მოქმედების შეზღუდვები.

აქ არ იწერება კოდის არქიტექტურა, API/SQL/Spanner-ის ტექნიკური დეტალები, ინფრასტრუქტურული ოპერაციები ან შიდა გადაწყვეტილებები. ასეთი მასალა ცალკე `gss-private-docs`-ში ინახება.

## ორგანიზება

ყველა დოკუმენტი პროდუქტისა და თემატიკის მიხედვითაა დაჯგუფებული `GSS Products`-ში. პროდუქტისგან დამოუკიდებელი საერთო გზამკვლევები ინახება `GSS Products/General`-ის თემატურ ქვესაქაღალდეებში (`data-retention`, `storage`, `search`, `tables`), ხოლო კონკრეტული პროდუქტების გზამკვლევები - შესაბამისი პროდუქტის საქაღალდეში.

### საერთო გზამკვლევები (`GSS Products/General`)

- **მონაცემების შენახვა (`data-retention`):**
  - [ორგანიზაციის მონაცემები შეძენილი მეხსიერების გადაუხდელობისას](<GSS Products/General/data-retention/organization-nonpayment.md>) - შეძენილი მეხსიერების ვადა და თავისუფალი ადგილი, 90-დღიანი გაფრთხილებები, შვიდივე პროგრამის გათიშვა, 7-დღიანი აღდგენა და საბოლოო ფიზიკური წაშლა.
- **მეხსიერება (`storage`):**
  - [მეხსიერების გამოყენების დათვლა](<GSS Products/General/storage/storage-usage.md>) - მიმოხილვის გვერდის მაჩვენებლები, მონაცემებისა და მიმაგრებული ფაილების მოხმარება, შეძენის ბიჯი, საერთო გადახდის ანგარიშის განაწილება და ფაილების ატვირთვის ლიმიტები.
- **ძებნა (`search`):**
  - [საძიებო ფრაზის საერთო წესები](<GSS Products/General/search/search-phrase-rules.md>) - ველის მითითება, პირობების გაერთიანება (`და` / `ან`), რიცხვითი შედარებები, ბრჭყალები და ჩადგმული ძებნა.
- **ცხრილები (`tables`):**
  - [ცხრილში ჩანაწერების მონიშვნა](<GSS Products/General/tables/row-selection.md>) - ერთი ჩანაწერის, `Shift`-დიაპაზონისა და ყველა ჩატვირთული ჩანაწერის მონიშვნა მაუსითა და კლავიატურით.

### ვებ-სუპერფინი და სუპერფინი (`GSS Products/SuperFin`)

- **მონაცემების შენახვა (`data-retention`):**
  - [ვებ-სუპერფინის მონაცემების შენახვა უმოქმედობისას](<GSS Products/SuperFin/data-retention/organization-inactivity.md>) - ვებ-სუპერფინის აქტივობის 12-თვიანი ვადა, გაფრთხილებები, უმოქმედობისგან დაცვის მონიშვნა, 3-თვიანი შეხსენება, ავტომატური გათიშვა და აღდგენა.
- **ძებნა (`search`):**
  - [ვებ-სუპერფინი: ძებნის ზოლი და კლავიატურა](<GSS Products/SuperFin/search/search-bar.md>) - მთავარი საძიებო ზოლი, კლავიატურის მალსახმობები, ძებნის გასუფთავება და დამახსოვრებული ისტორია;
  - [ვებ-სუპერფინი: ანგარიშთა გეგმის, საწყისი ნაშთებისა და ბრუნვის ძებნა](<GSS Products/SuperFin/search/search-accounts.md>) - ანგარიშთა გეგმის, საწყისი ნაშთების, ბრუნვის თანხობრივი ველებისა და კონტაქტით ჩადგმული ძებნის წესები;
  - [ვებ-სუპერფინი: საბუთების ძებნა](<GSS Products/SuperFin/search/search-documents.md>) - საბუთების პირდაპირი და გატარების ველები, ანგარიშსა და კონტაქტზე ჩადგმული ძებნა და შეცვლილი/წაშლილი საბუთების რეჟიმი;
  - [ვებ-სუპერფინი: RS ანგარიშ-ფაქტურების ძებნა](<GSS Products/SuperFin/search/search-rs-invoices.md>) - RS ანგარიშ-ფაქტურების ტექსტური, რიცხვითი და სტატუსის მიხედვით ძებნა.
- **სუპერფინის ზოგადი გზამკვლევები (`general`):**
  - [SuperFin - ზოგადი გზამკვლევი (სარჩევი)](<GSS Products/SuperFin/general/README.md>);
  - [პროგრამის აღწერა და შესაძლებლობები](<GSS Products/SuperFin/general/description.md>);
  - [ინსტრუქციები და სასწავლო კურსი](<GSS Products/SuperFin/general/instructions.md>);
  - [გადმოწერა და საინსტალაციო ინსტრუქცია](<GSS Products/SuperFin/general/downloads.md>);
  - [ფასები და მომსახურების პირობები](<GSS Products/SuperFin/general/prices.md>).

### კონტაქტები (`GSS Products/Contacts`)

- [კონტაქტის შეყვანა და რედაქტირება](<GSS Products/Contacts/contact-input.md>) - პიროვნების, ორგანიზაციისა და ბანკის ბარათების შევსება, ველები და დაკავშირებული ჩანაწერები;
- [კონტაქტების ძებნა](<GSS Products/Contacts/search-contacts.md>) - პიროვნებების, ორგანიზაციებისა და ბანკების ძებნა, საძიებო ველები და ჩადგმული კავშირები;
- [კომუნიკაციის ისტორიის ძებნა](<GSS Products/Contacts/search-communication-history.md>) - კომუნიკაციის ისტორიის ჩანაწერების ძებნა და ფილტრაცია.

### მხარდაჭერები (`GSS Products/Supports`)

- [Q&A საბუთები - როლები და წვდომა](<GSS Products/Supports/qa-documents-roles-and-access.md>) - ცოდნის ბაზის საბუთების მართვის როლები და წვდომის წესები.

### გაყიდვები (`GSS Products/Sales`)

- [გაყიდული სერვისების სასიცოცხლო ციკლი (სარჩევი)](<GSS Products/Sales/Sold Services Lifecycle/README.md>):
  - [ძებნა და ფილტრები](<GSS Products/Sales/Sold Services Lifecycle/01-search-and-filters.md>);
  - [შექმნა, კავშირები და გადახდა](<GSS Products/Sales/Sold Services Lifecycle/02-create-connections-and-payment.md>);
  - [ვადები, აღდგენა და წაშლა](<GSS Products/Sales/Sold Services Lifecycle/03-lifecycle-terms-restore-and-delete.md>);
  - [როლები და უფლებები](<GSS Products/Sales/Sold Services Lifecycle/04-roles-and-permissions.md>);
  - [თანმხლები ინფორმაცია, ისტორია და მოქმედებები](<GSS Products/Sales/Sold Services Lifecycle/05-accompanying-info-history-and-actions.md>).

### GSS ტესტები (`GSS Products/GSS Tests`)

- [GSS ტესტები - სრული სახელმძღვანელო და სარჩევი](<GSS Products/GSS Tests/README.md>);
- [კონცეფცია და საგანმანათლებლო მოდელი](<GSS Products/GSS Tests/overview.md>) - „შპარგალკა / წყარო საბუთი“, შეცდომების როლი და წვდომის უფლებები;
- [როგორ გამოვიწეროთ ტესტები](<GSS Products/GSS Tests/how-to-subscribe.md>) - კატალოგი, ძებნა და გამოწერის მართვა;
- [ტესტის გავლის პროცესი და რანერი](<GSS Products/GSS Tests/test-runner-and-cheatsheet.md>) - „შპარგალკის“ გამოყენება, შემოწმება და ავტომატური რეჟიმი;
- [SuperFin-ის სწავლა ტესტებით](<GSS Products/GSS Tests/superfin-learning-guide.md>) - პრაქტიკული ქეისი და ყოველდღიური სასწავლო რუტინა;
- [FAQ და პრობლემების მოგვარება](<GSS Products/GSS Tests/faq-and-troubleshooting.md>) - ხშირად დასმული კითხვები, შეცდომების მთვლელი და რჩევები.
