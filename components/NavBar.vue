<template>
     <header class="header">
        <nav class="navbar">
            <NuxtLink to="/" class="logo font-bold fonted"><img src="@/assets/logo.webp"></NuxtLink>
            <ul class="nav-items flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0 hidden md:block">
            <NuxtLink to="/"><li class="text-black hover:text-indigo-400">Accueil</li>           </NuxtLink>
            <NuxtLink to="/PlanVélo"><li class="text-black hover:text-indigo-400">Le plan vélo</li> </NuxtLink>
            <NuxtLink to="/InfosVélo"><li class="text-black hover:text-indigo-400">Infos vélo</li>   </NuxtLink>
            <NuxtLink to="/ContactPage"><li class="text-black hover:text-indigo-400">Contact</li>    </NuxtLink>
            </ul>
            <button class="hamburger" :class="{active:navOpen}" @click="navOpen=!navOpen" >
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
            </button>
        </nav>
        

 <div id="sidemenu">
    <transition name="translateX">
      <nav v-show="navOpen">
        <div class="sidemenu__wrapper">
          <ul class="sidemenu__list">
            <li class="sidemenu__item"><NuxtLink to="/">Accueil</NuxtLink></li>
            <li class="sidemenu__item"><NuxtLink to="/PlanVélo">Le plan vélo</NuxtLink></li>
            <li class="sidemenu__item"><NuxtLink to="/InfosVélo">Infos vélo</NuxtLink></li>
            <li class="sidemenu__item"><NuxtLink to="/ContactPage">Contact</NuxtLink></li>
          </ul>
        </div>
      </nav>
    </transition>
  </div>
</header>
  <!-- 

    <header class="header">
        <nav class="navbar">
            <a href="#" class="nav-logo">WebDev.</a>
            <ul class="nav-menu" v-show="navOpen">
                <li class="nav-item">
                    <a href="#" class="nav-link">Services</a>
                </li>
                <li class="nav-item">
                    <a href="#" class="nav-link">Blog</a>
                </li>
                <li class="nav-item">
                    <a href="#" class="nav-link">About</a>
                </li>
                <li class="nav-item">
                    <a href="#" class="nav-link">Contact</a>
                </li>
            </ul>
            <button class="hamburger" v-on:click="navOpen=!navOpen" v-bind:class="{active:navOpen}">
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
            </button>
        </nav>
</header>
    <div class="bg-white">
        <nav class="nav-container container px-4 py-4 mx-auto md:flex md:justify-between md:items-center">
                <div class="flex items-center justify-between">
                <NuxtLink to="/" class="w-2/3 font-bold fonted"><img src="@/assets/logo.webp"></NuxtLink> 
                </div>
    
        <ul class="nav-items flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
            <NuxtLink to="/"><li class="text-black hover:text-indigo-400">Accueil</li>           </NuxtLink>
            <NuxtLink to="/PlanVélo"><li class="text-black hover:text-indigo-400">Le plan vélo</li> </NuxtLink>
            <NuxtLink to="/InfosVélo"><li class="text-black hover:text-indigo-400">Infos vélo</li>   </NuxtLink>
            <NuxtLink to="/ContactPage"><li class="text-black hover:text-indigo-400">Contact</li>    </NuxtLink>

            <i class="fas fa-bars" @click="showMenu()"> </i> // Hamburger icon with click method
        </ul>
        </nav>
    </div>
    Comment -->
    </template>
    <script>
 export default {
  data() {
    return {
        navOpen: false,
      };
    },
  method: {
    // a computed getter
    togle() {
      // `this` points to the component instance
      this.showMenu = !this.showMenu;
    }
}
 }

    </script>
    <style  lang="scss" scoped>

    .logo {
        width: 125px;
    }

    @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,500;1,400&display=swap');
    #sidemenu {
	nav {
		width: 100%;
		// height: calc(100% - #{$headerHeight} - #{$footerHeight});
		background: white;
		position: fixed;
		top: 115px;
        height: 400px;
		left: 0;
        display: flex;
        align-items: center;
        justify-content: center;
		z-index: 99;
		// box-shadow: 2px 0 3px$grey-6;
		// overflow-y: scroll;
	}

	.sidemenu {
		&__btn {
			display: block;
			width: 50px;
			height: 50px;
			background: grey;
			border: none;
			position: relative;
			z-index: 100;
			appearance: none;
			cursor: pointer;
			outline: none;

			span {
				display: block;
				width: 20px;
				height: 2px;
				margin: auto;
				background: white;
				position: absolute;
				top: 0;
				bottom: 0;
				left: 0;
				right: 0;
				transition: all .4s ease;

				&.top {
					transform: translateY(-8px);
				}

				&.bottom {
					transform: translateY(8px);
				}
			}
			&.active{
				.top {
					transform: rotate(-45deg);
				}
				.mid{
					transform: translateX(-20px) rotate(360deg);
					opacity: 0;
				}
				.bottom {
					transform: rotate(45deg);
				}
			}

		}

		&__wrapper {
      padding-top: 50px;
    }

		&__list {
			padding-top: 50px;
      list-style:none;
      padding: 0;
      margin: 0;
		}

		&__item {
			a {
        text-decoration: none;
				line-height: 1.6em;
				font-size: 1.6em;
				padding: .5em;
				display: block;
				color: black;
				transition: .4s ease;

				&:hover {
					background: lightgrey;
					color: dimgrey;
				}
			}
		}
	}
}

.translateX-enter{
	transform:translateX(-200px);
	opacity: 0;
}

.translateX-enter-active,.translateX-leave-active{
	transform-origin: top left 0;
	transition:.2s ease;
}

.translateX-leave-to{
	transform: translateX(-200px);
	opacity: 0;
}


    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    
    html {
        font-size: 62.5%;
        font-family: 'Roboto', sans-serif;
    }
    
    li {
        list-style: none;
    }
    
    a {
        text-decoration: none;
    }

    .header{
    border-bottom: 1px solid #E2E8F0;
    }

    .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 1.5rem;
    }
    
    .hamburger {
    display: none;
}

.bar {
    display: block;
    width: 25px;
    height: 3px;
    margin: 5px auto;
    -webkit-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
    background-color: #101010;
}

.nav-menu {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-item {
    margin-left: 5rem;
}

.nav-link{
    font-size: 1.6rem;
    font-weight: 400;
    color: #475569;
}

.nav-link:hover{
    color: #482ff7;
}

.nav-logo {
    font-size: 2.1rem;
    font-weight: 500;
    color: #482ff7;
}

@media only screen and (max-width: 768px) {
    .nav-menu {
        position: fixed;
        left: -100%;
        top: 5rem;
        flex-direction: column;
        background-color: #fff;
        width: 100%;
        border-radius: 10px;
        text-align: center;
        transition: 0.3s;
        box-shadow:
            0 10px 27px rgba(0, 0, 0, 0.05);
    }

    .nav-menu.active {
        left: 0;
    }

    .nav-item {
        margin: 2.5rem 0;
        display: none;
    }

    .hamburger {
        display: block;
        cursor: pointer;
    }
    .hamburger.active .bar:nth-child(2) {
        opacity: 0;
    }

    .hamburger.active .bar:nth-child(1) {
        transform: translateY(8px) rotate(45deg);
    }

    .hamburger.active .bar:nth-child(3) {
        transform: translateY(-8px) rotate(-45deg);
    }


}
    
    </style>


  