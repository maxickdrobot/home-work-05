# Робота з простим сайтом
## HTML
### Меню сайту
```
<header class="header">
    <ul class="menu">
        <li class="menu__item">
            <a class="menu__link" href="#">
                Home
            </a>
        </li>
        <li class="menu__item">
            <a class="menu__link" href="#">
                Messages
            </a>
        </li>
        <li class="menu__item">
            <a class="menu__link" href="#">
                Music
            </a>
        </li>
        <li class="menu__item">
            <a class="menu__link" href="#">
                Settings
            </a>
        </li>
    </ul>
</header>
```
### Контент сайту
```
<main class="main">
            <section class="section hero">
                <h1 class="hero__title">Title of page</h1>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae numquam placeat sunt vitae iusto velit, doloremque modi nam, nihil voluptatibus illo eaque, inventore corporis. Eaque optio ipsa eveniet rerum eos iusto provident molestias alias quod laudantium cumque laboriosam, ad fugit nisi tenetur velit expedita mollitia autem vel aperiam aliquid dolore repellendus. Quia, amet enim maxime odio excepturi libero dolorem? Nemo, aut? Labore soluta mollitia modi vero nostrum corrupti officia ullam, inventore nesciunt quam vitae quidem beatae sapiente, aliquam fuga quia iusto, consectetur saepe obcaecati dolores quas! Esse exercitationem aut maiores accusantium ex corrupti aliquam pariatur veniam, eveniet ipsam commodi at magni error id molestiae! Aperiam dolore veritatis nemo eligendi mollitia illo magni consequatur, delectus quae minus ratione iure maiores vitae molestiae fugiat unde est veniam dolorum fugit error! Dolores quod distinctio tempora facere, ipsam maxime est debitis sed? Tempore natus incidunt vitae voluptatibus culpa provident perspiciatis quaerat est, omnis, quidem laboriosam nisi harum voluptatum eius. Saepe aliquam accusantium fugiat excepturi! Aliquam provident iusto, harum maiores perspiciatis consectetur neque ratione unde id veritatis atque dolore quae delectus assumenda quo ea numquam, dolor totam dignissimos aut corporis cupiditate? Tempore repellendus voluptatem explicabo deserunt beatae aperiam, corporis enim recusandae atque magnam. Veniam assumenda hic perferendis molestiae ab at ad nemo eius laudantium impedit autem soluta repudiandae repellat reprehenderit quas harum sunt iusto mollitia voluptatibus voluptates, optio delectus! Ducimus, architecto recusandae? Aut et veritatis aspernatur assumenda labore voluptate, quo illo dolore aliquid. Rem, placeat. Magni architecto molestiae officia quos blanditiis eum provident mollitia voluptatum, esse necessitatibus numquam quibusdam possimus doloribus voluptatibus assumenda non eaque voluptate dicta, omnis voluptates! Fugit harum praesentium nemo architecto laborum cum iste, soluta corrupti nesciunt rem? Veniam asperiores, porro possimus quod reprehenderit ipsam, atque enim, cumque aliquam culpa delectus. Molestias quis nobis in harum dignissimos, tenetur provident enim officiis quo quod temporibus architecto fugiat vel, corrupti repudiandae ab eum voluptatem asperiores necessitatibus? Sed earum exercitationem natus quo aspernatur, ducimus quasi illo, autem impedit fuga dolorum tenetur? Earum similique aliquid magni exercitationem amet quas adipisci sit laudantium, quisquam unde. Aliquam beatae ad eius architecto veniam. Nam aspernatur facere, sed, amet ea delectus nostrum minima sint alias, debitis atque deserunt repellat. Cumque laborum harum ipsam cum delectus eaque culpa rem, reprehenderit dignissimos aperiam quam atque voluptatibus pariatur sit. Rem sit delectus voluptatum enim animi ad doloremque, sed fuga iusto tempore labore dolores a reiciendis. Illum, fugiat dolor. Omnis doloremque illo amet cupiditate, recusandae quam culpa voluptas quae, repudiandae sit ad labore dignissimos excepturi fuga distinctio veritatis? Unde quidem ratione saepe cumque officia rerum voluptatum voluptatem voluptate doloremque aliquid minima tempora illo error cum illum repellat, voluptates iste sunt ipsum totam suscipit hic reiciendis quos. Dignissimos totam nobis cumque numquam cum inventore! Neque, ab dolore sequi veniam doloremque totam? Asperiores architecto enim, porro minima ad sequi? Ullam sunt vel illo quia inventore, explicabo id quas accusamus obcaecati minus saepe eveniet distinctio! At laboriosam obcaecati inventore, nesciunt reprehenderit facere aliquam nihil nulla fuga rerum, aliquid aperiam molestias, veritatis delectus suscipit magni molestiae quidem cum!
                </p>
            </section>
        </main>
```
## CSS
### Оформлення меню 
```
.header {
    display: flex;
    justify-content: center;
    width: 100%;
    margin: 10px;
    background-color: #2b2b30;
    border-radius: 10px;
}

.menu {
    display: flex;
}

.menu__item {
    position: relative;
    overflow: hidden;
    margin: 20px 30px;
    font-size: 22px;
}

.menu__link {
    line-height: 120%;
    text-decoration: none;
    color: white;
}
```
### Реалізація hover для меню
```
.menu__item::after {
    content: "";
    position: absolute;
    left: -100%;
    bottom: 0;
    width: 100%;
    height: 2px;
    background-color: white;
    transition: left 0.5s ease 0s;
}

.menu__item:hover::after {
    left: 0;
}
```
### Стилізація контенту сторінки
```
p {
    margin: 10px 0;
}

.hero__title {
    font-size: 54px;
    font-weight: bold;
}
```