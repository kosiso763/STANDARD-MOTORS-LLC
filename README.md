import React from "react";

export default function HomePage() {
  return (
    <div className="min-h-screen bg-white p-6 font-sans text-blue-900">
      <header className="bg-blue-100 shadow-md p-6 rounded-2xl mb-8">
        <h1 className="text-4xl font-bold">
          <span className="text-black">STANDARD</span>{" "}
          <span className="text-blue-800">MOTORS LLC</span>
        </h1>
        <p className="text-lg text-blue-700">Wholesale Dealer & Automotive Services</p>
      </header>

      <main className="grid gap-6">
        <section className="bg-blue-50 p-6 rounded-2xl shadow">
          <h2 className="text-2xl font-semibold text-blue-800 mb-2">About Us</h2>
          <p className="text-blue-700">
            STANDARD MOTORS LLC is your trusted partner in wholesale automotive sales and services.
            We specialize in delivering quality vehicles and reliable service to dealers and clients
            across the region.
          </p>
        </section>

        <section className="bg-blue-50 p-6 rounded-2xl shadow">
          <h2 className="text-2xl font-semibold text-blue-800 mb-2">Contact Information</h2>
          <ul className="text-blue-700 space-y-1">
            <li><strong>Owner:</strong> Henry Ihekuna</li>
            <li><strong>Phone:</strong> <a href="tel:4434499672" className="text-blue-600">443-449-9672</a></li>
            <li><strong>Email:</strong> <a href="mailto:standardmotorsllc.smi@gmail.com" className="text-blue-600">standardmotorsllc.smi@gmail.com</a></li>
            <li><strong>Address:</strong> 4 N Exeter Street, Baltimore, MD 21202</li>
          </ul>
        </section>

        <section className="bg-blue-50 p-6 rounded-2xl shadow">
          <h2 className="text-2xl font-semibold text-blue-800 mb-2">Our Services</h2>
          <ul className="list-disc list-inside text-blue-700 space-y-1">
            <li>Wholesale vehicle sales</li>
            <li>Automotive servicing & repairs</li>
            <li>Vehicle sourcing for dealerships</li>
            <li>Fleet maintenance services</li>
          </ul>
        </section>

        <section className="bg-blue-50 p-6 rounded-2xl shadow">
          <h2 className="text-2xl font-semibold text-blue-800 mb-4">Request a Service</h2>
          <form className="space-y-4">
            <div>
              <label className="block text-blue-700">Full Name</label>
              <input type="text" className="w-full p-2 rounded border border-blue-300" placeholder="Your name" />
            </div>
            <div>
              <label className="block text-blue-700">Email</label>
              <input type="email" className="w-full p-2 rounded border border-blue-300" placeholder="you@example.com" />
            </div>
            <div>
              <label className="block text-blue-700">Phone Number</label>
              <input type="tel" className="w-full p-2 rounded border border-blue-300" placeholder="(555) 555-5555" />
            </div>
            <div>
              <label className="block text-blue-700">Service Needed</label>
              <select className="w-full p-2 rounded border border-blue-300">
                <option>Wholesale Vehicle Purchase</option>
                <option>Repair & Maintenance</option>
                <option>Vehicle Sourcing</option>
                <option>Other</option>
              </select>
            </div>
            <div>
              <label className="block text-blue-700">Additional Details</label>
              <textarea className="w-full p-2 rounded border border-blue-300" rows="4" placeholder="Describe your request..."></textarea>
            </div>
            <button type="submit" className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700">
              Submit Request
            </button>
          </form>
        </section>
      </main>

      <footer className="mt-10 text-center text-blue-500 text-sm">
        &copy; {new Date().getFullYear()} STANDARD MOTORS LLC. All rights reserved.
      </footer>
    </div>
  );
}
