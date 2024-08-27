<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog Pessoal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 10px 0;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 10px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
        }

        main {
            padding: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Meu Blog Pessoal</h1>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="posts">
            <!-- Postagens serão inseridas aqui -->
        </section>
    </main>
    <footer>
        <p>© 2024 Meu Blog Pessoal</p>
    </footer>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const posts = [
                {
                    title: 'Minha Primeira Postagem',
                    content: 'Este é o conteúdo da minha primeira postagem no blog!'
                },
                {
                    title: 'Outra Postagem Interessante',
                    content: 'Aqui está mais um conteúdo interessante para compartilhar.'
                }
            ];

            const postsSection = document.getElementById('posts');

            posts.forEach(post => {
                const postElement = document.createElement('article');
                postElement.innerHTML = `
                    <h2>${post.title}</h2>
                    <p>${post.content}</p>
                `;
                postsSection.appendChild(postElement);
            });
        });
    </script>
</body>
</html>
