    <!-- Header -->
    <section id="header" class="wrapper">

        <!-- Logo -->
            <div id="logo">
                <!-- <h1><a href="index.html">Escape Velocity</a></h1> -->
                <h1>Bókasapp</h1>
                <p>Skilvirkt, einfalt, fljótlegt</p>
            </div>

        <!-- Nav -->
            <!-- <nav id="nav">
                <ul>
                    <li class="current"><a href="index.html">Home</a></li>
                    <li>
                        <a href="#">Dropdown</a>
                        <ul>
                            <li><a href="#">Lorem ipsum</a></li>
                            <li><a href="#">Magna veroeros</a></li>
                            <li><a href="#">Etiam nisl</a></li>
                            <li>
                                <a href="#">Sed consequat</a>
                                <ul>
                                    <li><a href="#">Lorem dolor</a></li>
                                    <li><a href="#">Amet consequat</a></li>
                                    <li><a href="#">Magna phasellus</a></li>
                                    <li><a href="#">Etiam nisl</a></li>
                                    <li><a href="#">Sed feugiat</a></li>
                                </ul>
                            </li>
                            <li><a href="#">Nisl tempus</a></li>
                        </ul>
                    </li>
                    <li><a href="left-sidebar.html">Left Sidebar</a></li>
                    <li><a href="right-sidebar.html">Right Sidebar</a></li>
                    <li><a href="no-sidebar.html">No Sidebar</a></li>
                </ul>
            </nav> -->

    </section>


<style>
    /* Header */

	#header {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-align-items: center;
		-webkit-align-items: center;
		-ms-align-items: center;
		align-items: center;
		-moz-justify-content: center;
		-webkit-justify-content: center;
		-ms-justify-content: center;
		justify-content: center;
		position: relative;
		height: 22em;
		background: url("/images/banner.jpg") center center;
		background-size: cover;
		padding: 0;
	}

		#header:before {
			content: '';
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			background: url("/images/overlay.png");
		}

		.homepage #header {
			height: 10em;
		}
</style>