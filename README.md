<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Creator AI Studio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta
    name="description"
    content="Creator AI Studio builds AI-powered tools, workflows, and educational content for digital creators."
  />
  <style>
    :root {
      --bg: #050509;
      --card: #11121a;
      --accent: #3ea6ff;
      --text: #f6f6f8;
      --muted: #a0a4b8;
      --border: #262738;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
        sans-serif;
    }

    body {
      background: radial-gradient(circle at top, #14162b 0, #050509 55%);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .wrapper {
      max-width: 960px;
      margin: 0 auto;
      padding: 32px 16px 64px;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 32px;
    }

    .brand {
      font-size: 1.4rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .tagline {
      font-size: 0.9rem;
      color: var(--muted);
    }

    main {
      display: grid;
      gap: 32px;
    }

    section {
      background: rgba(9, 10, 18, 0.92);
      border-radius: 18px;
      padding: 24px 20px;
      border: 1px solid var(--border);
      box-shadow: 0 18px 50px rgba(0, 0, 0, 0.4);
    }

    h1,
    h2,
    h3 {
      margin-bottom: 12px;
      font-weight: 600;
    }

    h1 {
      font-size: 1.9rem;
    }

    h2 {
      font-size: 1.3rem;
      border-bottom: 1px solid var(--border);
      padding-bottom: 6px;
      margin-bottom: 14px;
    }

    p {
      margin-bottom: 10px;
      font-size: 0.96rem;
    }

    ul {
      padding-left: 18px;
      margin-bottom: 10px;
      font-size: 0.95rem;
    }

    .pill {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      padding: 4px 10px;
      border-radius: 999px;
      background: rgba(15, 118, 255, 0.12);
      color: var(--accent);
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      margin-bottom: 10px;
    }

    .sms-card {
      border: 1px solid #1f2933;
      background: radial-gradient(circle at top left, #10182b 0, #070915 60%);
    }

    .form-row {
      display: flex;
      flex-direction: column;
      gap: 8px;
      margin-top: 10px;
      margin-bottom: 10px;
    }

    label {
      font-size: 0.9rem;
    }

    input[type="text"],
    input[type="email"] {
      padding: 10px 12px;
      border-radius: 10px;
      border: 1px solid var(--border);
      background: #05060d;
      color: var(--text);
      font-size: 0.95rem;
    }

    input[type="text"]:focus,
    input[type="email"]:focus {
      outline: 1px solid var(--accent);
      border-color: var(--accent);
    }

    .checkbox-row {
      display: flex;
      align-items: flex-start;
      gap: 8px;
      margin: 6px 0 12px;
      font-size: 0.85rem;
    }

    .checkbox-row input[type="checkbox"] {
      margin-top: 3px;
      accent-color: var(--accent);
    }

    .small-text {
      font-size: 0.78rem;
      color: var(--muted);
    }

    button {
      border: none;
      border-radius: 999px;
      padding: 9px 18px;
      font-size: 0.95rem;
      font-weight: 500;
      cursor: pointer;
      background: linear-gradient(135deg, #3ea6ff, #7b5cff);
      color: #050509;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.6);
    }

    button:hover {
      filter: brightness(1.05);
    }

    footer {
      margin-top: 28px;
      font-size: 0.8rem;
      color: var(--muted);
      text-align: center;
    }

    @media (min-width: 900px) {
      main {
        grid-template-columns: 1.1fr 0.9fr;
        align-items: flex-start;
      }

      .span-2 {
        grid-column: 1 / -1;
      }
    }
  </style>
</head>
<body>
  <div class="wrapper">
    <header>
      <div>
        <div class="brand">Creator AI Studio</div>
        <div class="tagline">AI workflows and tools for modern creators.</div>
      </div>
    </header>

    <main>
      <!-- Left column: overview + SMS -->
      <section>
        <div class="pill">About</div>
        <h1>Creator AI Studio</h1>
        <p>
          Creator AI Studio builds and tests AI-powered tools, workflows, and
          educational content for video creators, designers, and digital
          entrepreneurs. We experiment with practical AI systems for editing,
          automation, and production workflows.
        </p>
        <p>
          This site also provides an optional SMS channel for subscribers who
          want to receive time-sensitive updates, release alerts, and account or
          access notifications from Creator AI Studio.
        </p>
        <p class="small-text">
          SMS participation is completely optional and requires explicit
          consent. Details are explained below.
        </p>
      </section>

      <section class="sms-card">
        <div class="pill">SMS Alerts & Notifications</div>
        <h2>Join SMS Updates (Opt-In)</h2>
        <p>
          By opting in, you agree to receive informational SMS/MMS messages from
          Creator AI Studio. These may include:
        </p>
        <ul>
          <li>Account or access verification messages you request;</li>
          <li>Important service or platform updates;</li>
          <li>Release notices, workflow changes, or availability alerts;</li>
          <li>Occasional links or media relevant to these updates.</li>
        </ul>

        <!-- This is purely front-end markup; hook it to your backend or Twilio as needed -->
        <form>
          <div class="form-row">
            <label for="phone">Mobile phone number (US):</label>
            <input
              type="text"
              id="phone"
              name="phone"
              placeholder="+1 555 123 4567"
              required
            />
          </div>

          <div class="checkbox-row">
            <input type="checkbox" id="sms-consent" name="sms-consent" required />
            <label for="sms-consent">
              I agree to receive SMS and MMS messages from Creator AI Studio
              about account-related notifications, service updates, and
              informational alerts. I understand that I can reply
              <strong>STOP</strong> at any time to opt out, or
              <strong>HELP</strong> for assistance.
            </label>
          </div>

          <p class="small-text">
            By submitting this form, you confirm you are the owner or customary
            user of the provided mobile number and that you authorize Creator AI
            Studio to send you text messages at this number. Message and data
            rates may apply. Message frequency varies based on your interactions
            and requested updates. No third-party numbers are messaged. We do
            not sell or rent your phone number.
          </p>

          <button type="submit">Request SMS Enrollment</button>
        </form>
      </section>

      <!-- Bottom: Privacy + Terms -->
      <section class="span-2">
        <div class="pill">Compliance</div>
        <h2>Privacy Policy</h2>
        <p>
          Creator AI Studio respects your privacy. We collect only the
          information you voluntarily provide, such as your name, email address,
          and mobile phone number, when you fill out forms or interact with our
          services.
        </p>
        <p>
          If you opt in to SMS updates, your mobile number is used solely to
          deliver text messages as described on this page, including
          authentication codes you request, service notifications, and related
          informational messages. We do not sell or rent your personal
          information to third parties.
        </p>
        <p>
          We may share limited data with service providers (such as SMS
          delivery platforms) strictly for the purpose of sending messages and
          maintaining our services. These providers are contractually obligated
          to protect your information.
        </p>
        <p>
          You may opt out of SMS messaging at any time by replying
          <strong>STOP</strong> to any message from us. You may also contact us
          at
          <a href="mailto:contact@creatoraistudio.com"
            >contact@creatoraistudio.com</a
          >
          to request access, correction, or deletion of your information, where
          applicable.
        </p>
      </section>

      <section class="span-2">
        <h2>Terms of Service</h2>
        <h3>Use of the Site</h3>
        <p>
          Creator AI Studio provides educational content, experimental tools,
          and communication channels for creators. By using this site, you agree
          to use it only for lawful purposes and not to interfere with or
          disrupt the operation of the site or related services.
        </p>

        <h3>SMS Messaging Terms</h3>
        <p>
          By opting in to SMS messages, you agree to receive text messages at
          the mobile number you provide. Message frequency varies and may depend
          on your interactions and requested notifications. Message and data
          rates may apply. You can opt out at any time by replying
          <strong>STOP</strong> to any message. For assistance, reply
          <strong>HELP</strong> or email us at
          <a href="mailto:contact@creatoraistudio.com"
            >contact@creatoraistudio.com</a
          >.
        </p>
        <p>
          Delivery of SMS and MMS messages is subject to your mobile carrier and
          network conditions. We are not liable for delays or failures in
          message delivery.
        </p>

        <h3>Changes</h3>
        <p>
          We may update these terms or this policy from time to time. Any
          changes will be posted on this page with an updated effective date.
          Your continued use of the site or SMS services after changes are
          posted indicates your acceptance of the updated terms.
        </p>

        <h3>Contact</h3>
        <p>
          For any questions regarding this site, privacy, or SMS messaging,
          contact:
          <a href="mailto:contact@creatoraistudio.com"
            >contact@creatoraistudio.com</a
          >.
        </p>
      </section>
    </main>

    <footer>
      © <span id="year"></span> Creator AI Studio. All rights reserved.
    </footer>
  </div>

  <script>
    document.getElementById("year").textContent =
      new Date().getFullYear().toString();
  </script>
</body>
</html>
