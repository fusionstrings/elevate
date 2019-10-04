<style>

/* ===================================================================
 * 14. stats - (_layout.scss)
 *
 * ------------------------------------------------------------------- */
#stats {
	background: #001835;
	padding-top: 7.2rem;
	padding-bottom: 4.8rem;
	text-align: center;
}

#stats .row {
	max-width: 1440px;
}

#stats .stat {
	min-height: 17.4rem;
	padding-bottom: 1.5rem;
}

#stats .icon-part {
	position: relative;
	padding-bottom: 2.1rem;
}

#stats .icon-part::after {
	content: "";
	display: block;
	width: 80px;
	height: 1px;
	background: rgba(249, 218, 79, 0.5);
	position: absolute;
	bottom: 0;
	left: 50%;
	margin-left: -40px;
}

#stats .icon-part i {
	font-size: 6rem;
	color: #f9da4f;
}

#stats .stat-count {
	color: #FFFFFF;
	font-size: 3.6rem;
	margin-top: 1.2rem;
	margin-bottom: 0;
	font-weight: var(--font-weight-medium);
	color: white;
}

#stats .stat-title {
	color: rgba(255, 255, 255, 0.3);
	font-size: 1.4rem;
}

/* ------------------------------------------------------------------- 
 * responsive:
 * stats 
 * ------------------------------------------------------------------- */
@media only screen and (max-width:1024px) {
	#stats .stat:nth-child(n) {
		border-left: 1px solid rgba(255, 255, 255, 0.05);
		padding-bottom: 1.5rem;
	}

	#stats .stat:nth-child(3n+1) {
		border: none;
	}

}

@media only screen and (max-width:768px) {
	#stats .stat:nth-child(n) {
		border-left: 1px solid rgba(255, 255, 255, 0.05);
	}

	#stats .stat:nth-child(2n+1) {
		border: none;
	}

}

@media only screen and (max-width:600px) {
	#stats .stat:nth-child(n) {
		border: none;
	}

}

</style>
<!-- stats
   	================================================== -->
<section id="stats" class="count-up">
  <div class="row">
    <div class="col-twelve">
      <div
        class="block-1-6 block-s-1-3 block-tab-1-2 block-mob-full stats-list">
        <div class="bgrid stat">
          <div class="icon-part">
            <i class="icon-pencil-ruler" />
          </div>

          <h3 class="stat-count">110</h3>

          <h5 class="stat-title">Awesome Projects</h5>
        </div>
        <!-- /stat -->

        <div class="bgrid stat">
          <div class="icon-part">
            <i class="icon-location-user" />
          </div>

          <h3 class="stat-count">9050</h3>

          <h5 class="stat-title">Clients Served</h5>
        </div>
        <!-- /stat -->

        <div class="bgrid stat">
          <div class="icon-part">
            <i class="icon-rewards-medal-1" />
          </div>

          <h3 class="stat-count">210</h3>

          <h5 class="stat-title">Awards Received</h5>
        </div>
        <!-- /stat -->

        <div class="bgrid stat">
          <div class="icon-part">
            <i class="icon-alien" />
          </div>

          <h3 class="stat-count">123</h3>

          <h5 class="stat-title">Crazy Ideas</h5>
        </div>
        <!-- /stat -->

        <div class="bgrid stat">
          <div class="icon-part">
            <i class="icon-coffee-mug" />
          </div>

          <h3 class="stat-count">1500</h3>

          <h5 class="stat-title">Coffee Cups</h5>
        </div>
        <!-- /stat -->

        <div class="bgrid stat">
          <div class="icon-part">
            <i class="icon-hourglass" />
          </div>

          <h3 class="stat-count">7200</h3>

          <h5 class="stat-title">Hours</h5>
        </div>
        <!-- /stat -->
      </div>
      <!-- /stats-list -->
    </div>
    <!-- /twelve -->
  </div>
  <!-- /row -->
</section>
<!-- /stats -->
