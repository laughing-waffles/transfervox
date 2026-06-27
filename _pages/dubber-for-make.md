---
title: Dubber for Make
description: Connect Dubber recordings, recording details, and data exports to Make scenarios.
offer_name: Dubber
offer_image: /assets/images/logos/dubber.svg
layout: landing-page
discount: false
permalink: /dubber-for-make/
---

<div class="ps-md-4 mb-4 bg-light p-5 shadow-sm rounded text-sm-center">
  <img src="{{ page.offer_image }}" class="img-fluid rounded-3" alt="Dubber logo" />
</div>

<div class="col-12 col-md-12">
  <div class="row align-items-center pb-6 pb-md-10">
    <div class="col-md-7">
      <h2 class="h1 mb-3">Use Dubber recordings in Make scenarios.</h2>
      <p class="lead">
        Dubber for Make connects your Dubber account to Make with Dubber Auth ID/Auth Token credentials. Build workflows from new recordings, fetch recording details, list recordings for backfill, and request Dubber data exports without maintaining a separate middleware service.
      </p>
      <p>
        The app is distributed as an invite-only Make community app for TransferVox-backed deployments. Customer connections live in the customer's Make organization and use the customer's own Dubber credentials.
      </p>
      <p>
        <a href="/request-demo/" class="btn btn-primary me-3">Request install access</a>
        <a href="#setup" class="btn btn-outline-primary">View setup steps</a>
      </p>
    </div>
    <div class="col-md-5">
      <div class="bg-light p-4 rounded-3 shadow-sm">
        <h3 class="h4">Included Make modules</h3>
        <ul class="mb-0">
          <li>New Recording Occurred trigger</li>
          <li>Get Recording Details</li>
          <li>List Recordings</li>
          <li>Create Data Export</li>
          <li>Create Data Export Job</li>
          <li>List and Get Data Exports</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="row align-items-start pb-6 pb-md-10">
    <div class="col-md-4">
      <h3 class="h4">Credentials</h3>
      <p>
        Use your Dubber Auth ID and Auth Token for the target account. Do not send Auth Tokens through normal support channels.
      </p>
    </div>
    <div class="col-md-4">
      <h3 class="h4">Regions</h3>
      <p>
        Select the Dubber region that matches your account. Supported options include US, UK, UK1, EU, AU, CA, SG, JP, and Sandbox.
      </p>
    </div>
    <div class="col-md-4">
      <h3 class="h4">Ownership</h3>
      <p>
        Saved connections belong to your Make organization. GitHub Actions for TransferVox cannot refresh or maintain customer-owned Make connections.
      </p>
    </div>
  </div>

  <h2 id="setup" class="h3 mb-4">Setup Steps</h2>
  <div class="row align-items-start pb-6 pb-md-10">
    <div class="col-md-6">
      <h3 class="h4">Install the app</h3>
      <ol>
        <li>Request access to the invite-only community app.</li>
        <li>Open the install link while signed into the Make organization that should own the scenarios.</li>
        <li>Create a Dubber Auth ID/Auth Token connection and select your Dubber region.</li>
        <li>Add the Dubber modules to a scenario or import a starter blueprint.</li>
        <li>Run a controlled test before enabling production scheduling.</li>
      </ol>
    </div>
    <div class="col-md-6">
      <h3 class="h4">Prepare a test</h3>
      <ul>
        <li>Make organization and scenario id.</li>
        <li>Dubber region selected in the connection.</li>
        <li>Module name and sanitized Make error text.</li>
        <li>Whether Dubber profile verification succeeds outside Make.</li>
      </ul>
    </div>
  </div>

  <h2 class="h3 mb-4">Access And Support</h2>
  <div class="alert alert-warning" role="alert">
    <strong>Security note:</strong> Do not send Dubber Auth Tokens, Make API tokens, recording URLs, or customer recording metadata through normal support messages.
  </div>

  <h2 class="h3 mb-4">Support Boundaries</h2>
  <div class="row align-items-start">
    <div class="col-md-6">
      <h3 class="h4">No keep-alive scenario required</h3>
      <p>
        The current app uses Auth ID/Auth Token to mint new Dubber access tokens when Make needs them. Existing legacy connections should be replaced with Auth ID/Auth Token connections.
      </p>
    </div>
    <div class="col-md-6">
      <h3 class="h4">App support</h3>
      <p>
        App support is provided by the app publisher, not Make. Use the access request path for install help, scenario setup, and operational support.
      </p>
      <p>
        <a href="/request-demo/" class="btn btn-primary">Contact TransferVox</a>
      </p>
    </div>
  </div>
</div>
